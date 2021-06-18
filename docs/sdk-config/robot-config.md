# Robot Configuration

This section of the d.ASH SDK documentation provides details about the configuration file for the robot - `robot_config.json` - found in the folder `\dash-sdk\configs`. Information in this section includes variable and definitions used to configure the [d.ASH server](../index.md#dash-server).

### 2.1 ^^Config File^^
``` json
{
    "serverAddress" : "localhost:50051",
    "robotHostname" : "192.168.80.3",
    "username" : "<USERNAME>",
    "camList" : ["RealsenseCam"],
    "payloads" : [],
    "dataStateLogFolder" : "G:/Temp/logs",
    "ssl" : true,
    "fastServer" : false,
    "fastServerHostname" : "localhost:7777",
    "secureDefaultToken" : false,
    "testMode" : true,
    "withAudio" : true,
    "realSenseConfig" : {
        "test" : true,
        "testFilenames" : ["../../test_videos/nus_left.mp4", "../../test_videos/nus_center.mp4","../../test_videos/nus_right.mp4"],
        "flipOptions" : {
            "0" : [false, false],
            "1" : [true, true],
        "2" : [false, false]
        },
        "baseWidth" : 640,
        "baseHeight" : 480,
        "codec" : "video",
        "width" : 320,
        "height" : 240,
        "bitrate" : 3600000
    }
}
```
<p>&nbsp;</p>

### 2.2 ^^Definitions^^

#### 2.2.1 Main

- **`serverAddress`** : Sets address of the spotServer in `<HOSTNAME>:<PORT>` format.
- **`robotHostname`** : Sets hostname of the Spot to connect to robot's IP.
- **`username`** : Sets username for d.ASH server credentials.
- **`camList`** : Sets a list of cameras active for the current session.
---
- **`payloads`** : Optional payloads list.
- **`dataStateLogFolder`** : Sets folder to write out the recorded msgpack data of the robot.
- **`ssl`** : Enables secure SSL messaging and encryption.
- **`testMode`** : Enables the Spot server to enter into test mode.
- **`withAudio`** : Enables audio streaming playback.

---
#### 2.2.2 Intel RealSense Configuration

- **`test`**: Enables simulation of camera streaming via provided custom mp4 video files specified as a list in `testFilenames`.
- **`testFilenames`**: List of test files.
- **`flipOptions`**: Specify how each camera flips long the x-axis and y-axis following the format `{"index" : [x-flip, y-flip]}`
---
- **`baseWidth`**: Sets processing width of the camera stream. 
- **`baseHeight`**: Sets the processing height of the camera stream. 
!!! tip "Video will be processed at this base resolution before being resized via `width` and `height`. Use these variables to change the actual processed resolution for power/efficiency considerations of the RealSense devices."
!!! note "Note that a minimum `baseWidth` of 640 and a minimum `baseHeight` of 360 is required."
- **`codec`**: Sets jpg/video options, with jpg being regular jpeg encoding and video using VP9 encoding. 
- **`width`**: Adjusts the final returned/resized width dimensions of the input camera stream
- **`height`**: Adjusts the final returned/resized height dimensions of the input camera stream
---

- **`bitrate`**:  This is the quality of the video encoding [only applies to video streaming]
!!! note "Note for HD Streaming, RealSense requires a high bitrate of 3600000."