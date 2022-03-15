# dC Pilot SDK

The dC Pilot SDK allows you to develop your own custom robot **Teleoperations** apps easily. You will need:

- C++14 compatible compiler ( VS2022 recommended )
- For AutoDrive: CUDA enabled GPU
- Windows 10

## 2.1 Discovering your robots

The first step you need to perform is to run the discovery service to find the robot you want registered in your fleet.

Here are the required includes:
```c++
#include <iostream>
#include <string>
#include <cxxopts.hpp>
#include <robotDiscovery.h>
#include <robotPilot.h>
#include <robotNode.h>
#include <unordered_map>
#include <functional>
#include <algorithm>
#include <chrono>
#include <thread>
```

Next, start the robot discovery service:
```c++
// Create the robot discovery service
auto rDiscovery = DashMicroSv::getRobotDiscovery();
// Login with your credetials
if (!rDiscovery->loginCloud(userName, pwd)) {
    std::cout << "ERROR! Invalid Login Credentials." << std::endl;
    return;
}
// Start the discovery
rDiscovery->startDiscovery();
```

You can now write a simple function like the one below to find the robot you want:
```c++
std::shared_ptr<DashMicroSv::RobotNode> findRobotWithName(
    DashMicroSv::RobotDiscovery& rDiscoveryIn, 
    const std::string& robotName, bool printList) 
{
    std::shared_ptr<DashMicroSv::RobotNode> retBot = nullptr;
    auto aliveBots = rDiscoveryIn.getAliveRobots();
    if (printList) {
        printRobotList(aliveBots);
    }

    for (const auto& aBot : aliveBots) {
        if (aBot->getName() == robotName) {
            retBot = aBot;
            break;
        }
    }
    return retBot;
}
```

So go ahead and retrieve your robot:
```c++
auto myRobotNode = findRobotWithName(*rDiscovery, "myRobot", true);
```

With your robot found, it is now time to construct the **Pilot** and control it via teleoperation commands.

## 2.2 Teleoperations

Use the robot you found in the previous section to construct your **Pilot**:

```c++
auto myPilot = std::make_shared(*rDiscovery, *myRobotNode);

// Now connect to the robot
if(!myPilot->connect()) {
    std::cout << "ERROR! Unable to connect to robot!" << std::endl;
    return;
}

```

### Game Loop Ticking, Moving Robot, Retrieving images

The recommended implementation to operate the robot is via a simple **Game Loop**. From there you can **tick** and send velocity commands as well as retrieve images from your robot. Some pseudo code of how
it will look like is presented below:

```c++
    std::vector<cv::Mat> camImgs;
    while(true) {

        // Retrieve camera images
        myPilot->tick(camImgs);
        ProcessCamImgs(camImgs);

        // Move robot
        float x = 0, y = 0, rot = 0;
        RetrieveJoystick(x, y, rot);
        myPilot->setFreeMoveVel(x, y, rot);

        // In MS
        Pause(1.0);
    }
```

This concludes the simple tutorial/writeup on how to use the Pilot SDK to teleoperate your own robots.
