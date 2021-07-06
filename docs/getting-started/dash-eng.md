# Interfacing d.ASH Autonomy Engine with ROS

This section of the d.ASH SDK documentation provides details about using ROS with the d.ASH autonomy engine. Described below are ROS topics, along with their type and functionality.

## 4.1 Publications

| Topic | Type | Function |
| ------- | ------- | ------- |
| **`/active_path`** | `nav_mgs/Path` | Returns current path being executed. |
| **`/image`** | `sensor_msgs/Image` | Returns sensor image. |
| **`/initial_pose`** | `geometry_msgs/PoseWithCovarianceStamped` | Returns initial pose estimate for localization. |
| **`/localization_status`** | `std_msgs/String` | Returns status of localization certainty. |
| **`/mcl_pose_marker`** | `visualization_msgs/Marker` | Returns current localization position. |
| **`/nearest_wpts`** | `visualization_msgs/Marker` | Returns nearest waypoints for the robot to follow. |
| **`/odom`** | `nav_msgs/Odometry` | Returns odometry reading. |
| **`/original_path`** | `nav_msgs/Path` | Returns original path before processing. |
| **`/particle_array`** | `geometry_msgs/PoseArray` | Returns localization particle certainty. |
| **`/tracking_wpt`** | `std_msgs/Float32MultiArray` | Returns nearest waypoints for the robot to follow. |

## 4.2 Subscriptions

| Topic | Type | Function |
| ------- | ------- | ------- |
| **`/cmd_vel`** | `geometry_msgs/Twist` | Accepts manual command velocity. |
| **`/imu`** | `sensor_msgs/Imu` | Accepts imu sensor data. |
| **`/initial_pose`** | `geometry_msgs/PoseWithCovarianceStamped` | Accepts initial pose estimate for localization. |
| **`/joy`** | `sensor_msgs/Joy` | Accepts joystick message. |
| **`/move_base_simple/goal`** | `geometry_msgs/PoseStamped` | Accepts final goal from RVIZ. |
| **`/odom`** | `nav_msgs/Odometry` | Accepts odometry reading. |
| **`/lidar_points`** | `sensor_msgs/PointCloud2` | Accepts lidar scan.|