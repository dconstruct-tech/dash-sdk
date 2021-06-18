# Setting Up d.ASH

As mentioned previously, the d.ASH consists of three main components - d.ASH server, d.ASH service, and d.ASH autonomy engine. This section of the d.ASH SDK documentation provides details about setting up the d.ASH server. Information in this section includes compiling, and testing.


### 4.1 ^^Installing d.ASH Dependencies^^

To install the remaining d.ASH dependencies using pip, the following [desktop dependencies](/setup/desktop-dep) must be set up prior:

- [ ] [Intel RealSense SDK 2.0](https://github.com/IntelRealSense/librealsense/releases/tag/v2.45.0)
- [ ] [ROS Melodic on Ubuntu 18.04](/desktop-dep/#12-ros-installation)
- [ ] [FFmpeg and others](https://www.ffmpeg.org/download.html)

If the above dependencies have been installed, proceed by running the following command to install the rest of the python packages:
```
python3.7 configLibs.py
```
Please ensure you are in the `\dash-sdk` directory before running. Following the instructions prompted by the terminal to proceed with installation.

--- 

### 4.2 ^^Setting up d.ASH Server^^

To set up the d.ASH server, you will need to configure the d.ASH server configuration file - `robot_config.json` - located in the folder `\dash-sdk\configs`. 

```
dash-sdk/
└─ configs/
    └─ robot_config.json
    └─ ...
```

Look under the [SDK Configuration](\sdk-config\robot-config) section to find out more about setting up `robot_config.json` for the d.ASH server. Then, to run the d.ASH server, execute the following command on your terminal:

``` python3
$ python3.7 ./dash_server.py robot_config.json
```

---

### 4.3 ^^Setting up d.ASH Service^^

To set up the d.ASH service, you will need to configure the d.ASH service configuration file - [`dash_service_config.json`](\sdk-config\rest-config) - located in the folder `\dash-sdk\configs`. 

```
dash-sdk/
└─ configs/
    └─ dash_service_config.json
    └─ ...
```

First, run `runrest` to see available IP address for your rest server:
```python
runrest
```
Pick the index of the IP address you like and append it to the `activeIPIdx` variable:
```
"activeIPIdx" : 1, # where '1' is the chosen IP address indec
```
Then, you will need to set your `preferredIP` address, that is, the IP address for the computer onboard your robot. This IP address will have precedence over `activeIPIdx`. Similarly, replace the default IP address with your preferred IP address:
```
"preferredIP" : "10.8.0.5",
```
Ensure that the IP address of the onboard computer is within the same subnet by the remote client. Lastly, you will need to change the `<PATH_OF_SDK>` of `cmdPath`. 
```
"cmdPath" : "<PATH>"
```

To do this, use `pwd` to print your current working directory path and replace `<PATH_OF_SDK>`. For example, if your current directory is `/home/dash_sdk/py_server`:

```
"cmdPath" : "/home/dash_sdk"
```

To test the d.ASH service, you'll need to run the d.ASH service by running the following command: 

``` python3
./robot_rest <PATH_TO_SDK>/configs/dash_service_config.json
```

Now that your d.ASH service is running, you can use our d.ASH Pilot app. To launch the  d.ASH Pilot app, simply search for it in your Windows search bar. Now, login to the system and connect to your robot to start controlling your robot. For more information on the d.ASH Pilot, refer to the [d.ASH Pilot guide]().


### 4.4 ^^Setting up d.ASH Autonomy^^

To set up the d.ASH autonomy, you will need to configure the d.ASH autonomy configuration file - [`auto_config.json`](/sdk-config/auto-config) - located in the folder `/dash-sdk/configs/`.

```
dash-sdk/
└─ configs/
    └─ auto_config.json
    └─ ...
```

Look under the [SDK Configuration](\sdk-config\robot-config) section to find out more about setting up `robot_config.json` for the d.ASH autonomy.

<!-- Then, using apt-get to install  following packages to set up the ROS Driver:
[TENTATIVE]
```
$ sudo apt install ros-melodic-hector-trajectory-server ros-melodic-realsense2-camera ros-melodic-velodyne ros-melodic-joy ros-melodic-octomap ros-melodic-dynamic-edt-3d ros-melodic-tf2 ros-melodic-serial* libgoogle-glog-dev git libssl-dev libusb-1.0-0-dev pkg-config libgtk-3-dev libglfw3-dev libgl1-mesa-dev libglu1-mesa-dev
$ sudo add-apt-repository ppa:joseluisblancoc/gtsam-develop
$ sudo apt update
$ sudo apt install libgtsam-dev
$ sudo apt-key adv --keyserver keys.gnupg.net --recv-key 6F3EFCDE
$ sudo apt update
$ sudo apt install librealsense2*
$ sudo apt install libudev-dev
$ sudo apt-get install libsecret-1-dev
``` -->

### 3.6 ^^Testing d.ASH Autonomy Engine^^
To test the d.ASH autonomy engine, run the executable below to start autonomy driver. Note to replace `<PATH_TO_SDK>` with your current working directory containing the d.ASH SDK:

```
./dash_autonomy <PATH_TO_SDK>/config/auto_config.json
```

To find your current working directory, use `pwd`. For example, if your directory is `/home/dash-sdk`, you would run the following command to test d.ASH autonomy:

```
./dash_autonomy /home/dash-sdk/config/auto_config.json
```

!!! tip "You will need to run d.ASH server before running d.ASH service and d.ASH automony."

On a seperate terminal, start a simple `roslaunch` test by running the following prompt, replacing `<PATH_TO_SDK>` with your current working directory containing the d.ASH SDK:

```
cd \launch
roslaunch <PATH_TO_SDK>\dash_sdk\launch\simple_joy.launch
```

Launch files have been prepared for setup - either with the [Velodyne VLP-16](\getting-started\config-connect\#21-velodyne-driver) lidar sensor or the [Ouster OS1-32](\getting-started\config-connect\#22-ouster-driver) lidar sensor. These lauch files can be found in under the `\dash-sdk\launch` folder. You can also create your own sensor launch files for your tests.