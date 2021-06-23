# Interfacing d.ASH Autonomy Engine with ROS

## 2.1 Publications

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

## 2.2 Subscriptions

| Topic | Type | Function |
| ------- | ------- | ------- |
| **`/cmd_vel`** | ??? | Returns manual command velocity. |
| **`/ext_auto_cmd_vel`** | ??? | Returns autonomous command velocity from external planner. |
| **`/imu`** | ??? | Returns |
| **`/initial_pose`** | `geometry_msgs/PoseWithCovarianceStamped` | Returns initial pose estimate for localization. |
| **`/joy`** | ??? | Returns joystick message. |
| **`/move_base_simple/goal`** | ??? | Returns final goal from RVIZ. |
| **`/odom`** | `nav_msgs/Odometry` | Returns odometry reading. |
| **`/lidar_points`** | ??? | Returns lidar scan.|