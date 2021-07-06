# d.ASH Autonomy Controller

As mentioned previously, the d.ASH autonomy controller is a GUI (graphical user interface) for the d.ASH SDK. It allows users to plot waypoints for autonomous navigation on maps, tracking and monitoring path planning. This section of the d.ASH SDK documentation provides details about setting up the d.ASH autonomy controller, including information on its respective components.

| d.ASH Autonomy Controller | Description |
| ------- | ------- |
| ![Screenshot](img/map.jpg){ align=left style="width:3000px"} | <font size="3"> Pair d.C Pilot with [d.ASH Autonomy Controller](/dash-sdk/dash-auto/UE-client) for remote autonomous operations. You'll be able to generate high quality real time 3D maps or launch point and click waypoint based missions. |

---
### 1.1 ^^Main Components^^


| Component | Description |
| ------- | ------- |
| ![Placeholder](img/main.png){ .center style="width:500px"} | <br> <font size="3"> (1) ^^Main toolbar^^: Used to open other menus.  <br><br> (2) ^^Slider^^: Used to move floor grid up and down. <br><br> 3) ^^Access mode^^: Used switch to mouse/keyboard mode. <br> (3) (a) ^^Navigation^^: The default mode uses the keys `WASD` to move camera and right click the mouse to zoom/tilt the camera. <br> (3) (b) ^^Waypoint creation^^: Used for adding waypoints to routes. <br><br> (4) ^^Floor grid^^ |

---

### 1.2 ^^Login^^

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/login.png#center){ .center style="width:500px"}| <br> <font size="3"> The login icon allow dConstruct users to log into the d.ASH autonomy controller using their cloud admin credentials. |

---

### 1.3 ^^Robot Connection^^

The robot connection icon allow users to connect/disconnect their respective robots to the d.ASH autonomy controller. 

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/robot-connect.png){ align=left style="width:500px"}| <font size="3"> (1) ^^Online pannel^^: Select from a list of robots that are online and ready to be used to connect to.  <br><br> (2) ^^Connected pannel^^: Select from a list of robots that you have connected to in the client to manipulate. <br><br> (3) ^^Add button^^: Press to connect to the robot selected in the online list to add the robot to the connected list. <br><br> (4) ^^Minus button^^: Press to disconnect from a robot in the connected list. |
| ![Screenshot](img/init.png#center){ align=left style="width:500px"}| <br> <font size="3"> When users first start the d.ASH SDK, they need to give an initial estimation of the robot's post on the map by configuring its `init pose`. <br><br> It tells the robot where its rough initial position is. To initialize `init pose`, draw the orange arrow by left clicking and drag the mouse on the floor grid.|

---

### 1.4 ^^Routes^^

The routes icon allow users to set routes for the robot to follow using waypoints. Add/remove waypoints to build your own custom routes.

#### 1.4.1 Route Controls

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/routes.png#center){ align=left style="width:350px"} | <font size="3"> (1) ^^Route name pannel^^: Enter route name to add. <br><br> (2) ^^Add button^^: Click to add route of given name. <br><br> (3) ^^Route selection pannel^^: Click to select a route. <br><br> (4) ^^Minus button^^: Press to disconnect from a robot in the connected list. <br><br> (5) ^^Waypoint button^^: Click to add waypoints to selected route. <br><br> (6) ^^Load/save button^^: Load/save all routes. <br><br> (7) ^^Segment pannel^^: Use keypad +/- to increment/decrement segment number. |

---

#### 1.4.2 Setting Up Routes

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/waypoint-1.png#center){ align=left style="width:800px"} | <font size="3"> To make a selected robot follow a selected route, add waypoints by clicking on the grid. Use `WASD` and right-click on the mouse to manipulate the view. |
| ![Screenshot](img/waypoint-2.png#center){ align=left style="width:500px"} <br> ![Screenshot](img/waypoint-3.png#center){: style="width:500px"} | <font size="3"> Once the waypoints have been set, exit waypoint mode by middle clicking the mouse. On the other hand, to remove a waypoint, click on the waypoint (selected waypoint change to the color orange), and press the `delete` ket to remove. |
| ![Screenshot](img/waypoint-4.png#center){ align=left style="width:500px"} | <font size="3"> You can also adjust the elevation of the grid by pressing the key `ctrl` and the mouse scroll moving the floor grid in waypoint mode. A waypoint is created when you click on grid, so, to create elevated waypoints, move grid up/down and then click.|

---

### 1.5 ^^Map Settings^^

The map settings icon allow users to adjust highpass, lowpass, UV Scale, and UV offset settings to customise the visuals of your map.

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/map.png#center){ align=left style="width:500px"} | <font size="3">  ^^Low pass slider^^: Voxels below this value is visible. Voxels in maps have elevation, and by lowering the low pass, voxels above the low pass will be cropped. |
| ![Screenshot](img/map-2.png#center){ align=left style="width:500px"} | <font size="3"> Notice that the ceiling voxels have now been cropped by reducing the low pass. |

---

### 1.6 ^^Layer Visibility^^

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/layer.png#center){ align=left style="width:500px"} | <font size="3">  The layer visibility icon allow users to toggle the visibility of various items on the map. |

---

### 1.7 ^^Load Scans^^

The load scans icon allow users to preview scans from the d.ASH Pack.

| Component | Description |
| ------- | ------- |
| ![Screenshot](img/load-scan.png#center){ align=left style="width:500px"} | <font size="3">  (1) ^^Vox downsample size pannel^^: Select your down sample size (in metres). A large value means lower quality, but faster loading. <br><br> (2) ^^Point clouds button^^: Pick loaded point clouds to toggle translucency.. |
| ![Screenshot](img/load-scan-2.png#center){ align=left style="width:500px"} | <font size="3">  Load scans in translucent mode. |