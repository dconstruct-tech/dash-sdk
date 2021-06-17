# ROS Driver
As mentioned, the ROS driver is a ROS node handles computational calls and sends control commands to the d.ASH server. It acts as an intermediate layer for ROS messages to be communicated with d.ASH server and unreal-clients through [gRPC](https://grpc.io/docs/what-is-grpc/introduction/).


### 5.1 ^^Update External Libraries^^ 

First, let's update the external libs, more specifically the `grpc_layer`, by executing the following commands:

```
$ git submodule update --init --recursive
$ git submodule update --remote --merge
```


### 5.2 ^^Installing Vcpkg^^

Vcpkg is a tool to manage C and C++ libraries on Windows, Linux and MacOS. Firtsly, you'll need to [install `vcpkg`](https://www.programmersought.com/article/92525780986/). Once installed, we need to use vcpkg to download the following packages to set up the ROS Driver:

```
$ cd ~/vcpkg
$ ./vcpkg install grpc:x64-linux
$ ./vcpkg install nlohmann-json:x64-linux
$ ./vcpkg install libsodium:x64-linux
$ ./vcpkg install msgpack:x64-linux
$ ./vcpkg install eigen3:x64-linux
$ ./vcpkg install opencv[world]:x64-linux
$ ./vcpkg install spdlog:x64-linux
$ ./vcpkg install pcl:x64-linux
```
Then, using apt-get to install  following packages to set up the ROS Driver:

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
```


### 5.3 ^^Configuration^^
Now, we need to place the [`auto_config.json`](/sdk-config/auto-config) into the folder `/dash-sdk/security/`.

  
### 5.4 ^^Running the Driver^^
Once compiled, run executable SDK to start autonomy driver, replacing `<PATH_TO_SDK>` with your current working directory containing the d.ASH SDK.

```
./dash_autonomy <PATH_TO_SDK>/config/auto_config.json
```
To find your current working directory, use `pwd`. For example, if your directory is `/home/dash-sdk`, you would run the following command:

```
./dash_autonomy /home/dash-sdk/config/auto_config.json
```