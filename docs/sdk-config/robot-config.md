# Robot Configuration

This section of the d.ASH SDK documentation provides details about the configuration file for the robot - `robot_config.json` - found in the folder `\dash-sdk\configs`. Information in this section includes variable and definitions used to configure the d.ASH server.

### 3.1 ^^Config File^^
``` json
{
    "server_address" : "localhost:50051",
    "robot_hostname" : "192.168.80.3",
    "username" : "<USERNAME>",
    "cam_list" : ["RealsenseCam"],
    "payloads" : [],
    "data_state_log_folder" : "G:/Temp/logs",
    "ssl" : true,
    "fast_server" : false,
    "fast_server_hostname" : "localhost:7777",
    "secure_default_token" : false,
    "test_mode" : true,
    "with_audio" : true,
    "real_sense_config" : {
        "test" : true,
        "test_filenames" : ["../../test_videos/nus_left.mp4", "../../test_videos/nus_center.mp4","../../test_videos/nus_right.mp4"],
        "flip_options" : {
            "0" : [false, false],
            "1" : [true, true],
        "2" : [false, false]
        },
        "base_width" : 640,
        "base_height" : 480,
        "codec" : "video",
        "width" : 320,
        "height" : 240,
        "bitrate" : 3600000
    }
}
```

---

### 3.2 ^^Definitions^^
#### 3.2.1 Main

| Variable | Definition |
| ------ | ------ |
| **`server_address`** | Sets address of the d.ASH server in `<HOSTNAME>:<PORT>` format. |
| **`robot_hostname`** | Sets hostname of the Spot to connect to robot's IP. |
| **`username`** | Sets username for d.ASH server credentials. |
| **`cam_list`** | Sets a list of cameras active for the current session. |
| **`payloads`** | Optional payloads list. |
| **`data_state_log_folder`** | Sets folder to write out the recorded msgpack data of the robot. |
| **`ssl`** | Enables secure SSL messaging and encryption. |
| **`test_mode`** | Enables the d.ASH server to enter into test mode. |
| **`with_audio`** | Enables audio streaming playback. |

---

#### 3.2.2 Intel RealSense Configuration

| Variable | Definition |
| ------ | ------ |
| **`test`** | Enables simulation of camera streaming via provided custom mp4 video files specified as a list in `test_filenames`. |
| **`test_filenames`** | List of test files. |
| **`flip_options`** | Specify how each camera flips long the x-axis and y-axis following the format `{"index" : [x-flip, y-flip]}`. |
| **`baseWidth`** | Sets processing width of the camera stream. Note that a minimum `baseWidth` of 640 is required. |
| **`baseHeight`** | Sets the processing height of the camera stream. Note that a  minimum `baseHeight` of 360 is required. |
| **`codec`** | Sets jpg/video options, with jpg being regular jpeg encoding and video using VP9 encoding. |
| **`width`** | Adjusts the final returned/resized width dimensions of the input camera stream. Video will be processed at this base resolution before being resized via `width` and `height`. Use these variables to change the actual processed resolution for power/efficiency considerations of the RealSense devices.
| **`height`** | Adjusts the final returned/resized height dimensions of the input camera stream. Video will be processed at this base resolution before being resized via `width` and `height`. Use these variables to change the actual processed resolution for power/efficiency considerations of the RealSense devices. |
| **`bitrate`** |  This is the quality of the video encoding. Note for HD Streaming, RealSense requires a high bitrate of 3600000. |