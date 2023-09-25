<p align="center"><img src="docs/img/d.ASH-Black.svg" width="25%" /><br><br></p>

-----------------

## Overview
**dConstruct d.ASH SDK** is a cross-platform library for autonomous robot navigation. Use the d.ASH SDK to develop applications for your own Spot from Boston Dynamics or any other robot you wish. 

> :pushpin: For more information on the d.ASH SDK documentation, please refer to the [latest documentation release](https://dconstruct-tech.github.io/dash-sdk/).

## What’s included in the SDK:
| What | Description |
| ------- | ------- |
| **d.ASH Server** | The d.ASH server acts as the main server responsible for sending control commands to the robot. At the same time, the d.ASH server also broadcasts secured data to any given remote systems.|
| **d.ASH Autonomy Engine** | The d.ASH Autonomy Engine is the autonomy backend code that runs on the edge of the robot. It empowers the robot with robust multi-terrain (indoor and outdoor) autonomous navigation capabilities. It handles secure communication between automony engine and the remote autonomy controller. |
| **d.ASH Autonomy Controller** | The d.ASH autonomy controller is the GUI (graphical user interface) for the d.ASH autonomy engine. It enable users to monitor and have full remote control of autonomy by allowing users to plot waypoints and activate autonomy on a fleet of robots. Stream real-time data via a secure connection between robots and the controller using 4G or 5G. |

## Ready to Test!
There are two mission scripts available for general-purpose task execution and manipulation which can be found under the folder [`\missions`](https://github.com/dconstruct-tech/dash-sdk/tree/master/missions). Execute these mission scripts - `short_test.mission` and `office_test.mission` - sequentially to control your Spot in any way you like. If you'd like to write your own missions, there are a total of 5 different types of missions:

| Function | Description |
| ------- | ------- |
| `clearmission()` | The function `clearmission()` allows users to clear all previous missions in history.|
| `pause(int)` | The function `pause(int)` allows users to stop Spot from walking and pause for (int) number of seconds. |
| `capture(int)` | The function `capture(int)` allows users to capture an image using their camera ID. |
| `endWayPoint()` | The function `endWayPoint()` allows users to send and follow a series of waypoints defined before `endWaypoint()` is called. |
| `moveToPoint(float, float, float)` | The function `moveToPoint(float, float, float)` allows users to move to a specified point `(x, y, z)` using a global planner. |

To run your mission, execute the following command in your terminal, replacing `<IP>:<PORT>` with your IP address : port number and `<MISSION_FILE_PATH>` with the directory path to your mission file:
```
./send_mission   <IP>:<PORT>   <MISSION_FILE_PATH>
```
For example:
```
./send_mission   10.0.0.3:3000   C:/Users/dc/Desktop/dash_sdk/missions/short_test.mission
```

## License
This project is licensed under the [BSD 2-Clause License](LICENSE).
Copyright 2021 dConstruct Technologies Pte Ltd.


©2021 [dConstruct Technologies](https://www.dconstruct.co/). Designed and Engineered in Singapore.