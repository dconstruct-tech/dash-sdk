# Configuring Sensors
## 2.1 Velodyne Driver

The [Velodyne Driver](http://wiki.ros.org/velodyne_driver) is a driver in the ROS package that provides basic device handling for Velodyne 3D LIDAR sensors.

### 2.1.1 ^^Setting Up on Sensor^^
By default, the Velodyne LIDAR sensor IP address is factory set on default value `192.168.1.201`. The d.ASH SDK will assume the default Velodyne IP address.

### 2.1.2 ^^Setting Up on Personal Computer^^
You'll need to configure a static IP address for your computer to use an address within the range `192.168.1.XXX` where `XXX` may be any integer from 2 to 254, except 201 (which is the LIDAR’s IP). For example, an appropriate static IP address for your compute could be `192.168.1.100`. 

## 2.2 Ouster Driver

### 2.2.1 ^^Setting Up on Sensor^^
By default, the Ouster LIDAR sensor IP address is factory set on your IPv6/IPv4 link-local address. The addresses lie within the block `169.254.0.0` to `169.254.255.255`. To change the static IP address for Ouster, refer to the [Ouster Documentation](https://data.ouster.io/downloads/software-user-manual/software-user-manual-v2p0.pdf). It is recommended to set up your own static IP address. 

### 2.2.2 ^^Setting Up on Personal Computer^^

You'll need to configure a static IP address for your computer to use an address within the range `192.0.2.XXX` where `XXX` may be any integer from 2 to 254. For example, an appropriate static IP address for your compute could be `192.0.2.123`. 


You will need to go into the folder `/dash_sdk/launch` and execute the following command, replacing `<PATH_TO_SDK>` with the directory containing the `/dash_sdk/`:
```
cd /dash_sdk/launch/
catkin_make 
echo "source <PATH_TO_SDK>/dash_sdk/launch/devel/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

Now, let's test your lidar sensors. To test the Velodyne VLP-16 lidar sensor, run the following command:
```
cd dash_sdk/launch
roslaunch autonomy_velodine.launch
```
To test the Ouster OS1-32 lidar sensor, run the following command:
```
cd dash_sdk/launch
roslaunch autonomy_ouster.launch
```
Finally, to check if the ROS messages are published correctly, in another terminal, run the following command:
```
rostopic echo /velodyne_points
```