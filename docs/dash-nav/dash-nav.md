<style>
    a:hover {
        text-decoration: underline;
    }

    .instructions-div {
        display: flex; 
        align-items: center; 
        margin-right: 10px;
    }

    .instruction-circle {
        width: 18px;
        height: 18px;
        background-color: #ff3300;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        font-size: 12px;
        font-weight: bold;
        border: 1px solid #ff3300;
    }

    .table_contents {
        color: black;
        text-decoration: none; 
    }

    .table_contents:hover {
        text-decoration: underline;
    }
</style>

# d.ASH Nav

### Introduction

| ![Screenshot](img/dash-nav-first-image.png){ align=center style="width:400px"} |

Welcome to the d.ASH Nav application user guide! Whether you're using a mobile device or computer desktop for robot operations, we've got you covered. To access the user guide for your Android mobile devices, please refer to <a href="#section2">Section 2</a> in this page. For desktop usage, please turn to <a href="#">Section 3</a>.

Now, let's delve into the functionalities that d.ASH Nav offers for seamless robot operations and the respective steps for each of them!

### Table of Contents
This is the list of sections that can be found in our user guide. For quick access, simply click on the Section that you would like to see.

##### <a class="table_contents" href="#section1">1. Application Functionalities</a>

##### <a class="table_contents" href="#section2">2. d.ASH Nav for Android</a>
* <a class="table_contents" href="#section2_1">2.1 Installation guide</a>
* <a class="table_contents" href="#section2_2">2.2 Your account</a>
* <a class="table_contents" href="#section2_3">2.3 A Quick Start Guide</a>

##### <a class="table_contents" href="#section3">3. Welcome to d.ASH Nav!
* <a class="table_contents" href="#section3_1">3.1 Setting up your robot</a>
* <a class="table_contents" href="#section3_2">3.2 Loading in your map file </a>

##### <a class="table_contents" href="#section4">4. View Tab</a>
* <a class="table_contents" href="#section4_1">4.1 Adjusting map view</a>

* <a class="table_contents" href="#section4_2">4.2 Map View Configurations</a>
   
* <a class="table_contents" href="#section4_3">4.3 Good and bad map visualizations</a>

##### <a class="table_contents" href="#section5">5. Ready Tab</a>
* <a class="table_contents" href="#section5_1">5.1 Live camera streaming</a>
* <a class="table_contents" href="#section5_2">5.2 Manually controlling your robot</a>
* <a class="table_contents" href="#section5_3">5.3 Localizing your robot</a>

##### <a class="table_contents" href="#section6">6. Plan Tab </a>
* <a class="table_contents" href="#section6_1">6.1 Creating your route</a>
    * <a class="table_contents" href="#section6_1_1">6.1.1 Setting route via waypoint</a>
    * <a class="table_contents" href="#section6_1_2">6.1.2 Setting route via manual control</a>
    * <a class="table_contents" href="#section6_1_3 ">6.1.3 BLK scanning</a><br>

        - <a class="table_contents" href="#section6_1_4_1">6.1.4.1 BLK Scan Configurations (LiDAR Scan Quality/Image Capture Mode)</a>
        * <a class="table_contents" href="#section6_1_4_2">6.1.4.2 Auto generation of BLK scan points</a>
        * <a class="table_contents" href="#section6_1_4_3">6.1.4.3 Manually selecting BLK scan points</a>
        
* <a class="table_contents" href="#section6_2">6.2 Editing and deleting your routes</a>
* <a class="table_contents" href="#section6_3">6.3 Running your routes</a>

##### <a class="table_contents" href="#section6">7. Offline Mode </a>
---

<div id="section1"></div>
### 1. Application Functionalities

d.ASH Nav is the platform for autonomous control of your robots. Being seamlessly integrated in the d.ASH Fleet Management workflow, you can enjoy easy planning and deployment of your robots for various use cases. d.ASH Nav allows you to plot waypoints for autonomous navigation on maps, tracking and monitoring path planning, as well as overall monitoring of your robots.

An internet connection from your robot is required. Should you require d.ASH Nav without an internet connection, please contact us <a href="#">here</a> for more details.

<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Pilot</p>
</div>

Our Pilot framework offers high-performance, low-latency, long-range remote operations. It allows you to take manual control of your robots at any time, from any distance, and in any environment.

<div style="display: flex; align-items: center;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Live Video Streaming</p>
</div>

Our ultra-high-speed data streaming enables Pilot to stream live video feeds from robots, facilitating operation in environments with weak network infrastructure. Stay connected with minimal latency, you can take control across the country with d.ASH Nav.

<div style="display: flex; align-items: center;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Waypoint Autonomy</p>
</div>

d.ASH Nav determines the real-time location of connected robots within millimetres. Just drop and add waypoints like markings on a map to automated patrol routes all thanks to d.ASH Nav’s seamless UI.

<div style="display: flex; align-items: center;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Enhanced Safety and Risk Mitigation</p>
</div>

The software’s intelligent decision-making capabilities enable robots to make informed choices to avoid obstacles and optimize their routes, mitigating potential risks and enhancing overall safety. This not only protects the robots themselves but also minimizes the risk of accidents or collisions with humans and other objects in the environment.

Now, let's explore how to make the most out of d.ASH Nav on your devices.

---

<div id="section2"></div> 
### 2. d.ASH Nav for Android
This comprehensive guide will walk you through setting up the application and provide detailed insights into every function of the d.ASH Nav Mobile App. Additionally, you'll find step-by-step instructions on how to seamlessly control your robots directly from your mobile device.

<div id="section2_1"></div> 
### 2.1 Installation guide
Before installing, ensure that your mobile device meets the minimum system requirements. 

#### Minimum system requirements
Android Tablet with support for OpenGL ES 3.2
Operating System: Android Version 13 | Tiramisu  | API Level 33 
Screen Size: No smaller than 10.5 inches
Processor: Snapdragon 888 chip on the Samsung Galaxy Tab S8 

To find a list of compatible Android devices, click [here]().



<div id="section2_2"></div> 
### 2.2 Your account
Login to d.ASH Nav with your given credentials.
Your login details can be found in the email we have sent you. If you encounter any difficulties logging in, please contact us [here]().
<img src="img/login.jpg" style="width: 400px; margin-top: 10px;" />


<div id="section2_3"></div>
### 2.3 Quick Start Guide  
The following section provides a step-by-step guide to help you record and set your desired route for the robot to follow, as well as apply BLK scans. Additional features offered by d.ASH Nav are listed in the subsequent sections.

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Connect to your robot and load your map into the application. </p></div><font size="3"><font size="2"> Refer to <a href="#section3_1">Section 3.1</a> and <a href="#section3_2">Section 3.2</a> for a guide for your robot and map respectively.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Navigate into the ready tab and select localise. </p></div><font size="3"><font size="2"> Refer to <a href="#section5_3">Section 5.3</a> for a guide to giving your robot a good initial pose estimate. |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Inside the plan tab, select add new route and give your route a name.</p></div><font size="3"><img src="img/add-route-button.jpg" style="width: 300px; margin-top: 10px;"/><br><font size="2"> Choose a name that is both memorable and descriptive. |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Press the record route button at the bottom right to record your route by moving the robot.</p></div><font size="3"><img src="img/record-route-button.jpg" style="width: 50px; margin-top: 10px;" /><br><font size="2"> Alternatively, you can refer to <a href="#section6_1_2">Section 6.1.2</a> to learn how to record your route by manually plotting waypoints onto the map. |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Use the joysticks to drive your robot along your preferred route. </p></div><font size="3"><font size="2"> Be sure to change the recording intervals and make use of the add point buttons while recording your route. For example, at sharp turns, you can change the recording interval lower to about 1 metre. |
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;">Once you are satisfied with your route, select save recorded route.   </p></div><font size="3"><font size="2"> Or, if you would like to restart, select discard route at the bottom.  |
| <div class="instructions-div"><div class="instruction-circle">7</div><p style="margin: 0; margin-left: 5px;">Optional: Choose the points in your route where you would like your robot to apply a BLK scan. </p></div><font size="3"><font size="2"> Refer to <a href="section6_1_4">Section 6.1.4</a> for a full guide on choosing waypoints to apply BLK scans.|
| <div class="instructions-div"><div class="instruction-circle">8</div><p style="margin: 0; margin-left: 5px;">In the list of routes, press the route you just created and select set route located at the bottom of the screen. </p></div><font size="3"> |
| <div class="instructions-div"><div class="instruction-circle">9</div><p style="margin: 0; margin-left: 5px;">Head back to the ready tab and change the control mode at the bottom to auto. </p></div><font size="3"><img src="img/control-mode-auto-toggle.png" style="width: 300px; margin-top: 10px;"/><br><font size="2"> Well done! Your robot is now running on your recorded route that you have made.   |


---

<div id="section3"></div>
### 3. Welcome to d.ASH Nav Mobile!

After signing into your account, you'll be directed to the main page where you need to load your robot and map files in order to get started.
<img src="img/dash-nav-home-page.jpg" style="width: 1000px; margin-top: 10px;">

<div id="section3_1"></div>
### 3.1 Connecting to your robot

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Turn on your robot</p></div><font size="3"><font size="2"> Typically, robots are activated automatically by attaching a battery and pressing the Power ON button/switch. However, for robots that require activation through software, like the Boston Dynamics Spot, please refer to the detailed instructions provided on the robot manufacturer's website for specific guidance. |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Connect to the robot's WiFi network</p></div><font size="3"><font size="2"> Open your mobile device's settings app, click on Connections -> Wi-Fi, and then connect to the network of your robot. After a successful connection, you should see 'Connected without internet' below the Wi-Fi network. If no network is found, it indicates that your robot may not have been turned on properly. |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Return to the application. On the left hand side, click here to select your robot.</p></div><font size="3"><font size="2"><img src="img/select-robot.png" style="margin-top: 10px;" /> |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Choose the robot that you intend to use.</p></div><font size="3"><font size="2"> If your robot is not found, try to hard restart your robot or contact us <a href="#">here</a> for support. |

<div id="section3_2"></div>
### 3.2 Loading in your map file 

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Ensure that you have your map file.</p></div><font size="3"><font size="2"> If you do not have one, please refer to our <a src="#">d.ASH Pack guide</a> to create your map. |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">On the left hand side, click on this button to select your map.</p></div><font size="3"><font size="2"><img src="img/select-map-button.png" style="margin-top: 10px;" />|
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Select the map that you intend to use.</p></div><font size="3"><font size="2"><img src="img/select-map-panel.jpg" style="margin-top: 10px;" />|


Your robot and map file has now been imported. 
<img src="img/both-imported-view.png" style="margin-top: 10px;" />

Select the menu icon on the top right hand corner to open up the options menu, where all functions and configurations are found.<br> 


The following sections will go over the functions in the <a href="#section4">View</a> tab, which is responsible for changing the view of your map, as well as the <a href="#section6">Plan</a> and <a href="#section5">Ready</a> tabs which are responsible for all robot operations. 

<img src="img/option-panels.png" style="width: 300px;"/>

---

<div id="section4"></div>
### 4. View Tab
The view tab contains options for changing the view and configuring the map that was imported into the application.

<div id="section4_1"></div>
#### 4.1 Adjusting your view of the map
<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Pinch to zoom in or zoom out</p>
</div>
<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Swipe with one finger to adjust view angle</p>
</div>
<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">Swipe with two fingers to move around</p>
</div>

<img src="img/adjust-view.gif" />

Select this button on the top left corner to reset view to default. 
<img src="img/reset-view.png" style="margin-top: 10px;"/>

<div id="section4_2"></div>
#### 4.2 Map View Configurations
##### Clipping 
Move the points on the range slider to adjust how much floor/ceiling is shown on the map of your application. 
<img src="img/clipping.png" style="width: 600px; margin-top: 10px;" />

##### Contours
Toggle on and off or adjust the contour level to change the amount of detail in data points. 
Toggle on and off or adjust the contour level to adjust contour sensitivity. 
<img src="img/contour.png" style="width: 600px; margin-top: 10px;"/>

<div id="section4_3"></div>
#### 4.3 Example of a bad map visualization
The View Tab allows you to customise your map-viewing experience within the application. It provides you with the flexibility to configure the settings according to your preferences. While keeping the default settings is perfectly acceptable, it's recommended to adjust the thumbs in a way that ensures the floor of the map is visible, the ceiling is hidden, and artefacts remain visible for optimal viewing.

<img src="img/bad-visualization.jpg" style="width: 600px; ">

The ceiling covers the entire map and you are unable to see the artifacts below, hence this is a bad map visualization. To make this visualization better and clearer, let's adjust the ceiling knob lower until the ceiling is hidden.

<img src="img/adjust-ceiling.gif" style="width: 600px; ">

This way, we can better see where our robot is located on the map when we run a route or control the robot.

---

<div id="section5"></div>
### 5. Ready Tab
Within this tab, you will find all the functions for managing the robot's live video streaming, manual controlling, and localization, which is essential for the Plan tab. 

<div id="section5_1"></div>
#### 5.1 Live video streaming 
To see your robot's camera view, select or toggle the camera options here. This can be found in the options menu on the right. 

<!-- <img src="img/camera-view.jpg" style="width: 800px;">  -->
<img src="img/camera-view.gif" style="width: 600px;">

You can also enlarge the camera view by pressing the enlarge button on the top left corner and adjust the size to your preference. 

<div id="section5_2"></div>
#### 5.2 Manually controlling your robot 

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">To move your robot, switch the control mode at the bottom of the application to manual mode.</p></div><fonst size="3"><img src="img/control-mode-toggle.png" style="width: 300px; margin-top: 10px;" /><br><font size='2'>Ensure that you are on the ready tab. |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;"> Use the joysticks to move the robot. </p></div><font size="3"><img src="img/manual-control-mode.jpg" style="width: 400px; margin-top: 10px;"/><font size="2"><br>The joystick on the left is used to move the robot front and backwards, while the right joystick is used to turn the robot left and right.|

<div id="section5_3"></div>
#### 5.3 Localizing your robot 

Before delving into the features in the planning tab, it is essential to establish an initial pose estimate to initiate the robot's localisation. Localisation is a crucial step for the robot to accurately determine its position within the provided point cloud map. This process is a prerequisite for enabling autonomy on the robot.

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">On the top of the right panel of the application, press the Localise button.</p></div><fonst size="3"><img src="img/localize-button.png" style="margin-top: 10px; width: 300px;"/><br><font size='2'>Ensure that you are on the ready tab. Here, you can also find your robot status and see information like the battery, localisation and stance.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Localise the robot by matching the point cloud of the current lidar scan to the map.</p></div><font size="3"><font size="2"> Press on the point of the map where the robot is located and drag it to the direction it is facing. Then, use the directional arrows to adjust the robot's LiDAR's point cloud to fit the map.<img src="img/localize-demo.gif" style="margin-top: 10px;"> Alternatively, you can use the rotation button to adjust and improve your pose estimate. <img src="img/localize_rotation.gif" style="margin-top: 10px;"/>|
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Bring down the plane of the map.</p></div><font size="3"><font size="2"> Using the slider on the left, adjust the map plane such that the floor of the map is now visible. |

Upon submitting the initial pose estimate, the robot will attempt to determine its current position on the map. During this process, there may be a momentary "jump" in the robot's position. Users are advised to wait for a few seconds to ensure that the robot stabilises and remains at the correct position.

Refer to the examples below for instances of successful robot localisation.
<img src="img\localisation.png" style="margin-top: 10px;"/>
The localisation of the robot is good when the robot's current LiDAR scan (white points) is aligned well to the map, meaning it has a good initial pose estimate. The localisation on the other two examples are bad as the LiDAR scan does not line up with the map, and the robot is in the wrong position. 

---

<div id="section6"></div>
### 6. Plan Tab
The plan tab is used for preparing routes for your robots to follow and apply BLK scans.

<div id="section6_1"></div>
#### 6.1 Creating your route
Before starting, ensure that you have our localised your robot to the map. Refer to <a href="#section5_3">Section 5.3</a> if you require a guide to localise your robot onto the map. <br>
At the bottom right corner of your screen, select on the 'App Route' button.

<img src="img/add-route-button.jpg" style="width: 300px;" />

Give your new route a name. Try to use a name that is descriptive and well labelled.
<img src="img/add-new-route.jpg" style="width: 250px; margin-top: 10px;" />

You will then be directed to the route edit view. Here, you will be able to add and remove waypoints, change the configurations of BLK scanning, and generate scanning points around the map.
<img src="img/set-route-view.jpg" style="margin-top: 10px;" />

<div id="section6_1_1"></div>
#### 6.1.1 Setting route by waypoints
<img src="img/set-route-buttons.jpg.png" style="width: 300px;" />

To set your route, you can do it by manually making waypoints for the robot to follow. To do this, select the Add Mode button at the bottom of the screen. 

<img src="img/selected-add-mode.jpg" style="width: 300px;" />

Plot the various points on the map that you want your robot to go. Ensure that the points are next to each other, avoiding any obstacles in the map and hence in real life.

<img src="img/setting-route-by-waypoint.gif" style="width: 400px;">

If you want to delete a waypoint, select the Remove Mode button, and click on the waypoints that you would like to delete. 
<img src="img/selected-remove-mode.png" style="width: 400px; margin-top: 10px;">
Once you are finished with manually plotting your route, select the Done button on the left of the mode buttons. 

<div id="section6_1_2"></div>
#### 6.1.2 Setting route via manual control of your robot
Add a new route and give it a name. Once you've created a new route, exit back to the routes page by pressing the done button. 
On the bottom right of your map screen, click on this button.
<img src="img/record-route-button.jpg" style="width: 55px; margin-top: 10px;"> 
You will now have to manually control your robot around the map to create the path. Use the joysticks and 'Add Point' buttons to make your route. 
<img src="img/record-route-view.gif">


After moving your robot, you should see a blue-coloured path being formed by the robot. This path is the route you will set for your robots to follow.

Once you are finished with setting your route, press 'Save Recorded Route' at the bottom of the screen and you will be directed back to the routes page with your new route saved. 

Now, you will be able to make your robot run the route you have created. Refer to <a href="#section6_3">Section 6.3</a>.

<div id="section6_1_3"></div>
#### 6.1.3 BLK Scanning
Before setting BLK scan points, you can configure your LiDAR configurations depending on your use case. 

<div id="section6_1_3_1"></div>
#### 6.1.3.1 BLK Configurations
##### LiDAR Scan Quality
LiDar Scan Quality is the rate of how fast the LiDar spins, with low being the slowest and high being the fastest. Adjusting the LiDar Scan Quality would affect the amount of generated data points in your point cloud map. 

<img src="img/lidar-scan-quality-options.jpg" style="width: 200px;" />
<div style="display: flex; align-items: center; margin-top: -30px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px; margin-top: 30px;">Low: Resulting point cloud map after scan will be least detailed but generation speed is much faster. Usually used in situations where the environment that you want to scan is simple and does not require much detail.</p>
</div>
<div style="display: flex; align-items: center; margin-top: -50px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px; margin-top: 30px">Medium: Resulting point cloud map after scan will have a satisfactory level of detail for most applications. This setting is suitable for environments that have a moderate level of complexity, where you want a reasonable level of detail without sacrificing scanning efficiency. </p>
</div>
<div style="display: flex; align-items: center; margin-top: -20px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px; margin-top: 3px;">High: Resulting point cloud map after scan will be very detailed but generation speed is much slower.</p>
</div>

##### Image Capture Mode
<img src="img/image-capture-mode-options.jpg" style="width: 200px;"/><br>
<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">None : Does not utilize the camera for capturing images.</p>
</div>
<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">LDR (Low Dynamic Range) : Details in shadows may be lost or details in highlights may be blown out.</p>
</div>
<div style="display: flex; align-items: center; margin-top: -15px;">
    <img src="img/pointer.png" alt="Functionality Icon" height="20">
    <p style="padding-top: 16px; padding-left: 10px;">HDR (High Dynamic Range) : More detail in both highlights and shadows can be captured. </p>
</div>


<div id="section6_1_3_2"></div>
#### 6.1.3.2 Auto generation of scan points
In this section, you can automatically generate BLK scanning points in your route based on the distance travelled by the robot.

To enable this feature, turn this option on and set a distance interval. If your set distance interval is two metres, the robot will run a BLK scan every two metres travelled on your route.
<img src="img/auto-generate-scan-points.gif" style="margin-top: 10px;" />
The blinking points on your map is where your robot will apply a BLK scan. 

<div id="section6_1_3_3"></div>
#### 6.1.3.3 Manually setting scan points
Select the Scan Mode button at the bottom of the screen, and press the waypoints where you want your robot to do a BLK scan. 
<img src="img/manual-select-scan-points.gif" style="margin-top: 10px;" />

<div id="section6_2"></div>
#### 6.2 Editing or deleting your routes
Navigate to the right-hand side, where you'll find a list of the routes you've created. To edit or delete any of these routes, press and hold on the desired route. This action will reveal options such as rename, copy, and delete at the bottom of the screen.
<img src="img/edit-route.gif" style="margin-top: 10px;" />

<div id="section6_3"></div>
#### 6.3 Running your routes
| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Select the route that you would like to run.</p></div><fonst size="3"><font size='2'>You can find your routes in the routes section of the plan tab.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Once select, press the Set Route button located at the bottom of the screen.</p></div><font size="3"><font size="2"><img src="img/run-route-view.png" style="margin-top: 10px;"> |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Switch to the ready tab.</p></div><fonst size="3"><font size='2'>|
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Switch the control mode to Auto.</p></div><fonst size="3"><font size='2'><img src="img/control-mode-auto-toggle.png" style="width: 300px; margin-top: 10px;" />|
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Your robot will now run and follow the route that you've created.</p></div><fonst size="3"><font size='2'>|

#### 7. Offline Mode

<br>
Enjoy using d.ASH Nav! If you require any support, please feel free to contact us <a href="#">here</a>. 