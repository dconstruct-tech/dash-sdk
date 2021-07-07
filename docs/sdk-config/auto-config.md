# Auto Configuration

This section of the d.ASH SDK documentation provides details about the configuration file for the robot - `auto_config.json` - found in the folder `\dash-sdk\configs`. Information in this section includes variable and definitions to configure autonomy.

### 4.1 ^^Config File^^

``` python
{ 
    "py_address"                            : "0.0.0.0:50051",
    "ue_address"                            : "0.0.0.0:50052",
    "ssl"                                   : true,
    "motion_planner"                        : true,
    "localization"                          : true,
    "sim_mode"                                : false,
    "send_data_gui"                         : true,
    "camera"                                : "RealsenseCam",
    "retrieveImg"                           : false,
    "map_name"                              : "office_lvl4",
    "pc_topic"                              : "velodyne_points",
    "odom_topic"                            : "odom",

    "controller":{
        "linear_window"                     : 0.5,
        "linear_min_v"                      : 0.0,
        "linear_max_v"                      : 0.8,
        "angular_max_w"                     : 3.142,
        "linear_max_a"                      : 1.0,
        "angular_max_a"                     : 5.0,
        "robot_width"                       : 0.4,
        "robot_length"                      : 1.0,
        "obstacle_cost_gains"               : 3.0,
        "speed_cost_gains"                  : 1.0,
        "goal_cost_gains"                   : 4.0,
        "angular_speed_cost_scaling_factor" : 0.1,
        "linear_num_window_steps"           : 50,
        "angular_num_window_steps"          : 30,
        "prediction_window"                 : 5.0,
        "costmap_size"                      : 20.0,
        "costmap_scale"                     : 0.1,
        "max_pc_height"                     : 0.2,
        "min_pc_height"                     : -0.5,
        "x_filter"                          :[-0.2, 0.2],
        "y_filter"                          :[-0.1, 0.1],
        "costmap_obs_inflation"             : 1.0,
        "occ_obs_deadzone"                  : 0.2,
        "dt"                                : 0.1,
        "visualise"                         : false
    },
    "state_estimator":{
        "initial_x"                         : -7.7, 
        "initial_y"                         : -14.5, 
        "initial_z"                         : 1.0, 
        "initial_w"                         : -0.177,     
        "kImuTopic"                         : "imu", 
        "kPoseTopic"                        : "mcl_pose",
        "ktfUpdate"                         : 0.02,
        "kStatusUpdate"                     : 1.0,
        "kLoggingUpdate"                    : 15.0,
        "kposeDiffmax"                      : 5.0, 
        "KUse_imu_ori"                      : false,
        "kBadCovThres"                      : 2.0,
        "kGoodCovThres"                     : 0.7,
        "kCovBadMax"                        : 10, 
        "kCovGoodtMax"                      : 5,
        "kFilter_z"                         : true,
        "klimit_min"                        : -0.3,
        "klimit_max"                        : 5.0 
    },
    "planner":{
        "lookAheadIndex"                    : 15,
        "enable_self_rotate"                : false,
        "self_rotation_speed"               : 0.5,
        "self_rotation_speed_final"         : 0.3,
        "dis_threshold"                     : 0.5,
        "theta_threshold"                   : 0.2,
        "cmd_Smoothing"                     : true,
    }
}
```

---

### 4.2 ^^Definitions^^
#### 4.2.1 Main 

| Variable | Definition |
| ------ | ------ |
| **`py_address`** | The address of the d.ASH server in the formal `<IP>:<PORT>`. |
| **`ue_address`** | The address of the GUI server in the formal `<IP>:<PORT>`. |
| **`ssl`** | Enables secure SSL messaging and encryption. |
| **`motion_planner`** | Enables autonomy motion planning. |
| **`localization`** |  Enables robot localisation, returning users position and orientation in relation to map. |
| **`sim_mode`** | Enables Spot odometry retrieval. |
| **`send_data_gui`** | Enables ability to send data to GUI server for visualisation. |
| **`camera`** | Camera active for the current session to retrieve data ie. *RealsenseCam, TestCam*. |
| **`retrieveImg`** | Enables image retrieval. |
| **`map_name`** | Map name used for autonomy (as mentioned in [File Organisation](/dash-sdk/getting-started/map-loading)). |
| **`pc_topic`** | ROS point cloud topic name for subscribing |
| **`odom_topic`** | ROS odometry topic name for subscribing. |
 
---

#### 4.2.2 Controller

!!! tip "For the following parameters, ensure the value is within limits of the robot as per its documentation."

| Variable | Definition |
| ------- | ------ |
| **`linear_window`** | Sets DWA (dynamic window approach) size. |
| **`linear_min_v`** | Sets minimum linear velocity for autonomy. | 
| **`linear_max_v`** | Sets maximum linear velocity for autonomy. |
| **`angular_max_w`** | Sets maximum angular velocity for autonomy. |
| **`linear_max_a`** | Sets maximum linear acceleration for autonomy. |
| **`angular_max_a`** | Sets maximum angular acceleration for autonomy. |
| **`robot_width`** | Reflects width of robot. |
| **`robot_length`** | Reflects the length of robot. |
| **`obstacle_cost_gains`** | Sets weight for an obstacle course based on the weighted sum of the map. |
| **`speed_cost_gains`** | Sets weight for speed cost. |
| **`goal_cost_gains`** |  Sets weight for goal cost. |
| **`angular_speed_cost_scaling_factor`** | Sets weight for angular velocity. Note that a higher value of the variable discourages the robot from turning. |
| **`linear_num_window_steps`** | Sets number of linear velocity values to consider. Note that a higher value of the variable slows down the computations. |
| **`angular_num_window_steps`** | Sets number of angular velocity values to consider. Note that a higher value of the variable slows down the computations. |
| **`prediction_window`** | Sets prediction horizion (in seconds). Note that a higher value of the variable slows down the computations. |
| **`costmap_size`** | Sets local costmap size (in meters). |
| **`costmap_scale`** | Sets scale to convert map from meter to pixels. |
| **`max_pc_height`** | Sets maximum point cloud height to be considered as an obstacle. |
| **`min_pc_height`** | Sets minimum point cloud height to be considered as an obstacle. Note that the point cloud height is measured from the center of the lidar. If the ground is detected, it will be considered as an obstacle. Therefore, set the minimum value to be above the ground. |
| **`x_filter`** | Sets vector of size 2 consisting the minimum and maximum x-value of point cloud to be removed. Do not remove too much from the point cloud filter as obstacles around the robot might not be considered. |
| **`y_filter`** | Sets vector of size 2 consisting the minimum and maximum y-value of point cloud to be removed. Do not remove too much from the point cloud filter as obstacles around the robot might not be considered. |
| **`costmap_obs_inflation`** | Sets inflation radius of obstacles to be considered in planning. Note that a higher value of the variable results in more conservative planning. |
| **`occ_obs_deadzone`** |Sets minimum distances from obstacles and robots for autonomy. |
| **`dt`** | Sets timestep. Note that a higher timestamp slows down the computation. |
| **`visualise`** | Enables visualisation of costmap. This is used only for debugging. |

---

#### 4.2.3 State Estimator
| Variable | Definition |
| ------- | ------ |
| **`initial_x`** | Sets initialization of x-axis for localizaition (in meters). | 
| **`initial_y`** | Sets initialization of y-axis for localizaition (in meters). |
| **`initial_z`** | Sets initialization of z-axis for localizaition (in meters). |
| **`initial_w`** | Sets initialization of orientation for localizaition. |
| **`kImuTopic`** | ROS IMU (Inertial Measurement Unit) topic name for subscribing. |
| **`kPoseTopic`** | Enables localization result. |
| **`ktfUpdate`** | Sets ROS tf publishing frequency. |
| **`kStatusUpdate`** | Sets localisation status of publishing frequency. |
| **`kLoggingUpdate`** | Sets data logging period. |
| **`kposeDiffmax`** | Sets the maximum distance between two consecutive pose estimation. |
| **`KUse_imu_ori`** | Enables IMU (Inertial Measurement Unit) or odom orientation for odometry estimation. If this variable is set to true, ensure `kImuTopic` is available. |
| **`kBadCovThres`** | Sets localization quality. |
| **`kGoodCovThres`** | Sets localization quality. |
| **`kCovBadMax`** | Sets localization quality. |
| **`kCovGoodtMax`** | Sets localization quality. |
| **`kFilter_z`** | Enables pass through filter application for localization. |
| **`klimit_min`** | Sets minimum range of pass through filter. |
| **`klimit_max`** | Sets maximum range of pass through filter. |

---

#### 4.2.4 Planner

| Variable | Definition |
| ------- | ------ |
| **`lookAheadIndexv`** | Sets look-ahead index from the nearest waypoint for path to follow. Note that a lower index slows down the movement of the robot. Similarly, a higher index results in the robot not follow path properly. |
| **`enable_self_rotate`** | Enables one round of rotation around the robot itself before performing autonomy. This is to ensure that localisation is working before starting autonomy. |
| **`self_rotation_speed`** | Sets angular velocity of robot to turn around itself before performing autonomy (in radiants/second). |
| **`self_rotation_speed_final`** | Sets angular velocity of robot to turn around itself after performing autonomy (in radiants/second). This ensures that the final orientation of robot aligns with its goal. |
| **`dis_threshold`** | Sets maximum euclidean distance from the robot to the final goal for destination to be considered having reached its goal. Note that a smaller threshold discourages the robot from determing if it has reached its goal. |
| **`theta_threshold`** | Sets maximum orientation distance from the robot to the final goal for destination to be considered having reached its goal. Note that a smaller threshold discourages the robot from determing if it has reached its goal. |
| **`cmd_Smoothing`** | Enables smoothing control commands. |

