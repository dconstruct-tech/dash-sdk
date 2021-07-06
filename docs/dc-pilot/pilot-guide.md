# DC Pilot Client

The dC pilot is a GUI (graphical user interface) for the d.ASH SDK. It encompasses interactive visual components for you to control your robot both manually and autonomously. Operate your robots safely and precisely, from any location with our reliable and high-performance  BVLOS (Beyond Vision Line of Sight) System with high quality video streams and responsive controls. This section of the d.ASH SDK documentation provides details about using the d.C Pilot Client.

--- 
### 1.1 Introduction

The pilot client allows you to operate your robots safely and precisely, from any location via its high-performance BVLOS (Beyond Vision Line of Sight) system. It is also equipped with high quality video streams and responsive controls for seamless naviation. The system can also be used for fleet management, to discover, monitor and control multiple robots anytime, anywhere with real time video streaming and data collection.


The vision auto-drive is another key feature of the d.C Pilot, using machine learning and computer vision to analyze and understand your robot's surroundings. This allows you to then plot and navigate complex, unstructured environments using just cameras. Some requirements before starting the d.C Pilot are: 

1. Nvidia GPU enabled PC
2. Joystick connected to the PC

---

### 1.2 ^^Main Controls^^

| Tutorial |
| ------- | 
| ![Screenshot](img/main-screen.png){ align=center style="width:800px"} | 
| <font size="3"> To **start** the robot from rest, apply pressure on the joystick. |
| <font size="3"> To **stop** the robot from moving, release your hold on the joystick. | 
| <font size="3"> To move the robot **forwards**, push front on the joystick. |
| <font size="3"> To move the robot **backwards**, pull back on the joystick. |
| <font size="3"> To turn the robot to the **left**, tilt left on the joystick. | 
| <font size="3"> To turn the robot to the **right**, tilt right on the joystick. |
| <font size="3"> To get the robot to **stand** or **sit**, click the `stand` or `sit` button under the Basic Control panel on the right side of the main screen. |
---

### 1.3 ^^Control Pannel^^

| Control Pannel |
| ------- | 
| ![Screenshot](img/panel.png#center){ align=left style="width:700px"}| 
| <font size="3"> (1)  &nbsp; Unmute the microphone to allow dual-communication between the pilot client and the robot.
| <font size="3"> (2)  &nbsp; Toggle between audio to broadcast speakers. |
| <font size="3"> (3)  &nbsp; Record videos in mp4 format.
| <font size="3"> (4)  &nbsp; Upload/download video recordings.
| <font size="3"> (5)  &nbsp; Configure settings for your preference ie. night mode.
| <font size="3"> (6)  &nbsp; Broadcast live video streaming using eith a RTSP server or an HSL server. |

---

### 1.4 ^^Basic Control^^

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/basic-control.png#center){ align=left style="width:200px"} | <font size="3"> (1) &nbsp; Monitor the joystick position with respect to your robot. Control the robot by pushing further on the joystick. <br><br> (2) &nbsp; Adjust the cruise control speed using the slider control or if your joystick has a secondary lever, push the lever to activate. <br><br> (3)  &nbsp; Activate auto-drive for your robot to switch to Smart AI Assisted Cruise Autonomy. <br> -  &nbsp; Use the `spacebar` shortcut key to activate auto-drive. <br>  -  &nbsp; Use the `z` shortcut key for your robot to take the next few possible left turns. <br>  -  &nbsp; Use the `x` shortcut key for your robot to return to forward position after turning left or right. <br>  -  &nbsp; Use the `c` shortcut key for your robot to take the next few possible right turns.

---

### 1.5 ^^Cameras^^

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/cameras.png#center){ align=left style="width:600px"} | <font size="3"> (1) &nbsp; Select from a list of cameras onboard Spot, which are automatically detected by the pilot client.  <br><br> (2) &nbsp; Adjust the order of cameras for a wider view scope. Ticking the flipped settings will adjust the camera orientation. <br><br> (3)  &nbsp; Activate human tracking for people detection and labelling. |