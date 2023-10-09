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

# d.ASH Nav Mobile

### Introduction

![d.ASH Nav](img/dash-nav-first-image.png){ align=center style="width:900px"} 

Welcome to the d.ASH Nav application user guide! Whether you're using a mobile device or computer desktop for robot operations, we've got you covered. Now, let's delve into the functionalities that d.ASH Nav offers for seamless robot operations and the respective steps for each of them!

---

<div id="#section1"></div>

### 1. Application Functionalities

d.ASH Nav is the platform for autonomous control of your robots. Being seamlessly integrated in the d.ASH Fleet Management workflow, you can enjoy easy planning and deployment of your robots for various use cases. d.ASH Nav allows you to plot waypoints for autonomous navigation on maps, tracking and monitoring path planning, as well as overall monitoring of your robots.

An internet connection from your robot is required. Should you require d.ASH Nav without an internet connection, please contact us [here](mailto:hello@dconstruct.co) for more details.

![Functionality Icon](img/pointer.png){ style="height:20px;" } Pilot

Control your robots manually with low latency and high performance at any time, from any location, and in any setting.

![Functionality Icon](img/pointer.png){ style="height:20px;" } Live Video Streaming

Use d.ASH Nav to stream live video camera feeds from your robots, facilitating operation in environments with weak network infrastructure. Stay connected with minimal latency and take control of your robot across the country with d.ASH Nav.

![Functionality Icon](img/pointer.png){ style="height:20px;" } Waypoint Autonomy

Empower your robots with d.ASH Nav's advanced route creation and optimization capabilities. Seamlessly set precise routes and execute BLK scans tailored to your unique use cases. Elevate your automation experience with our state-of-the-art Waypoint Autonomy feature.

![Functionality Icon](img/pointer.png){ style="height:20px;" } Enhanced Safety and Risk Mitigation

d.ASH Nav enables robots to make informed choices to avoid obstacles and optimize their routes, mitigating potential risks while running routes and enhancing overall safety. This not only protects the robots themselves but also minimizes the risk of accidents or collisions with humans and other objects in the environment.

Now, let's explore how to make the most out of d.ASH Nav on your devices.

---

<div id="section2"></div> 

### 2. d.ASH Nav for Android
This comprehensive guide will walk you through setting up the application and give you detailed insights into every function of the d.ASH Nav Android Application. Additionally, you'll find step-by-step instructions on how to control your robots directly from your devices and create routes for waypoint automation.

<div id="section2_1"></div> 

### 2.1 Installation Guide
Before installing, ensure that your mobile device meets the minimum system requirements. 

| Minimum System Requirements                             | Recommended System Requirements                           |
|--------------------------------------------------------|------------------------------------------------------------|
| Android Tablet with support for OpenGL ES 3.2           | Android Tablet with support for OpenGL ES 3.2             |
| Operating System: Android Version 13 \| Tiramisu \| API Level 33  | Operating System: Android Version 13 \| Tiramisu \| API Level 33  |
| CPU: Qualcomm SM7125 Snapdragon 720G (8 nm)             | CPU: Snapdragon 888 Chip on Samsung Galaxy Tab S8        |
| GPU: Adreno 618                                        | GPU: Adreno 730                                         |
| RAM: 4 GB                                             | RAM: 8 GB                                              |

<div id="section2_2"></div> 

### 2.2 Your Account
Login to d.ASH Nav with your given credentials.
If you encounter any difficulties with logging in, please contact us.
![Login View](img/login.jpg){ style="width: 400px; margin-top: 10px;" }


<div id="section2_3"></div>

### 2.3 Quick Start Guide  
The following section provides a step-by-step guide to help you record and set your desired route for the robot to follow, as well as perform BLK scans. Additional features offered by d.ASH Nav are listed in the subsequent sections.

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Connect to your robot and load your map into the application. </p></div><font size="3"><font size="2"> Refer to <a href="#section3_1">Section 3.1</a> and <a href="#section3_2">Section 3.2</a> for a guide for your robot and map respectively.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Localise your robot onto the map. </p></div><font size="3"><font size="2"> Refer to <a href="#section5_3">Section 5.3</a> for a guide to giving your robot a good initial pose estimate. |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Inside the 'Plan' tab, select 'Add Route' and give your new route a name.</p></div><font size="3">![Add Route Button](img/add-route-button-full.png){ style="width: 1000px; margin-top: 10px;" }<br><font size="2"> Choose a name that is both memorable and descriptive. |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Select the route you just created and press the 'Record Route' button at the bottom right to record your route by manually moving your robot.</p></div><font size="3">![Record Route Button](img/record-route-button.png){ style="width: 1000px; margin-top: 10px;"}<br><font size="2"> Alternatively, you can refer to <a href="#section6_1_2">Section 6.1.2</a> to learn how to record your route by manually plotting waypoints onto the map. |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Use the joysticks to drive your robot along your preferred route. </p></div><font size="3"><font size="2"> Be sure to change the recording intervals and make use of the 'Add Point' buttons while recording your route. For example, when turning the robot, you can lower down the recording interval to about 1 metre for a better route recording, or use the 'Add Point' button to plot waypoints close to each other in this turn.<br>![Record Route View GIF](img/record-route-view.gif){style="margin-top: 10px;"}|
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;">Once you are satisfied with your route, select 'Save Recorded Route'.   </p></div><font size="3"><font size="2"> Or, if you would like to restart, select discard route at the bottom.  |
| <div class="instructions-div"><div class="instruction-circle">7</div><p style="margin: 0; margin-left: 5px;">Optional: Choose the points in your route where you would like your robot to apply a BLK scan. </p></div><font size="3"><font size="2"> Refer to <a href="#section6_1_3_2">Section 6.1.3.2</a> for a full guide on choosing waypoints to perform BLK scans.|
| <div class="instructions-div"><div class="instruction-circle">8</div><p style="margin: 0; margin-left: 5px;">In the list of routes, press the route you just created and select 'Set Route' located at the bottom of the screen. </p></div><font size="3">![Set Route Full](img/set-route-full.png){style="width: 1000px; margin-top: 10px;"} |
| <div class="instructions-div"><div class="instruction-circle">9</div><p style="margin: 0; margin-left: 5px;">Head back to the 'Ready' tab and change the control mode at the bottom to 'Auto'. </p></div><font size="3">![Control Mode Auto Toggle](img/running-route-ready-tab.png){ style="width: 1000px; margin-top: 10px;" }<br><font size="2"> Well done! Your robot is now running on your recorded route that you have made.   |

If you do not have access to internet at the location where you want to run your robot processes, you can use [Offline Mode](#section7).

---

<div id="section3"></div>

### 3. Welcome to d.ASH Nav Mobile!

After signing into your account, you'll be directed to the main page where you need to load your robot and map files in order to get started.
![d.ASH Nav Home Page](img/dash-nav-home-page.jpg){ style="width: 1000px; margin-top: 10px;"}

<div id="section3_1"></div>

### 3.1 Connecting to your robot

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Turn on your robot.</p></div><font size="3"><font size="2"> Typically, robots are activated automatically by attaching a battery and pressing the Power ON button/switch. However, for robots that require activation through software, like the Boston Dynamics Spot, please refer to the detailed instructions provided on the robot manufacturer's website for specific guidance. |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Ensure that your device is connected to the internet.</p></div><font size="3"><font size="2">  |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Return to the application. On the left hand side, click on this button boxed in red to select your robot.</p></div><font size="3"><font size="2">![Select Robot](img/select-robot.png){style="margin-top: 10px;"} |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Choose the robot that you intend to use.</p></div><font size="3"><font size="2"> If your robot is not found, try to hard restart your robot or contact us for support. |

<div id="section3_2"></div>

### 3.2 Loading in your map file 

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Ensure that you have your map file.</p></div><font size="3"><font size="2"> If you do not have one, please refer to our [d.ASH Pack](https://dconstruct-tech.github.io/dash-sdk/dash-pack/dash-pack/) guide to create your map.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">On the left hand side, click on this button boxed in red to select your map.</p></div><font size="3"><font size="2">![Select Map Button](img/select-map-button.png){style="margin-top: 10px;"}|
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Select the map that you intend to use.</p></div><font size="3"><font size="2">![Select Map Panel](img/select-map-panel.jpg){style="margin-top: 10px;"}|

Your robot and map has now been loaded into d.ASH Nav. 
![Both Robot and Map Imported](img/both-imported-view.png){style="margin-top: 10px;"}

Select the 'Menu' icon on the top right hand corner to open up the options menu, where all functions and configurations are found.<br> 

The following sections will go over the functions in the <a href="#section4">View</a> tab, which is responsible for changing the view of your map, as well as the <a href="#section6">Plan</a> and <a href="#section5">Ready</a> tabs which are responsible for all robot operations. 

![Optional Panels](img/option-panels.png){ style="width: 300px;" } 

---

<div id="section4"></div>

### 4. View Tab
The view tab contains options for changing the view and configuring the map that was loaded into the application.

<div id="section4_1"></div>

#### 4.1 Adjusting your view of the map
![Functionality Icon](img/pointer.png){ style="height:20px;" } Pinch to zoom in or zoom out

![Functionality Icon](img/pointer.png){ style="height:20px;" } Swipe with one finger to adjust view angle

![Functionality Icon](img/pointer.png){ style="height:20px;" } Swipe with two fingers to move around the map

![Adjust View GIF](img/adjust-view.gif)

Select this button on the top left corner to reset view to default.<br>
![Reset View Button](img/reset-view.png){style="margin-top: 10px;"}

<div id="section4_2"></div>

#### 4.2 Map View Configurations
##### Clipping 
Move the points on the range slider to adjust how much floor/ceiling is shown on the map of your application.
![Clipping Visualisations](img/clipping.png){style="width: 600px; margin-top: 10px;" }

##### Contours
Toggle on and off or adjust the contour level to adjust contour sensitivity. 
![Contour Visualisations](img/contour.png){style="width: 600px; margin-top: 10px;"}

<div id="section4_3"></div>

#### 4.3 Example of a bad map visualization
The View Tab allows you to customise your map-viewing experience within the application. It provides you with the flexibility to configure the settings according to your preferences. While keeping the default settings is perfectly acceptable, it's recommended to adjust the thumbs in a way that ensures the floor of the map is visible, the ceiling is hidden, and artefacts remain visible for optimal viewing.
![Bad Visualisations Example](img/bad-visualization.jpg){style="width: 600px; margin-top: 10px;"}

The ceiling covers the entire map and you are unable to see the artifacts below, hence this is a bad map visualization. To make this visualization better and clearer, let's adjust the ceiling knob lower until the ceiling is hidden.
![Adjust Ceiling GIF](img/adjust-ceiling.gif){style="width: 600px; margin-top: 10px;"}

This way, we can better see where our robot is located on the map when we run a route or control the robot.

---

<div id="section5"></div>

### 5. Ready Tab
Within this tab, you will find all the functions for managing the robot's live video camera streaming, taking manual control of your robot, and localisation, which is essential for the 'Plan' tab. 

<div id="section5_1"></div>

#### 5.1 Live video streaming 
To see your robot's camera view, select or toggle the camera options here. This can be found in the options menu on the right. 
![Camera View GIF](img/camera-view.gif){style="width: 600px; margin-top: 10px;"}<br>
You can also enlarge the camera view by pressing the enlarge button on the top left corner and adjusting the size to your preference. 

<div id="section5_2"></div>

#### 5.2 Manually controlling your robot 
![Manual Control Mode Switch](img/control-mode-switch-page.png){style="width: 800px;"}

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">To move your robot, switch the control mode at the bottom of the application to 'Manual' mode.</p></div><fonst size="3"><font size='2'>Ensure that you are on the 'Ready' tab. |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;"> Use the joysticks at the bottom to move your robot. </p></div><font size="3"><font size="2">The joystick on the left is used to move the robot front and backwards, while the joystick on the right is used to turn the robot left and right. |

<div id="section5_3"></div>

#### 5.3 Localising your robot 

Before delving into the features in the planning tab, it is essential to establish an initial pose estimate to localise your robot. Localisation is a crucial step for the robot to accurately determine its position within the provided point cloud map. This process is a prerequisite for enabling autonomy on the robot.

| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Inside the options panel of the 'Ready' tab, press the 'Localise' button.</p></div><fonst size="3">![Localize Button](img/localize-button.png){style="margin-top: 10px; width: 1000px;"}<br><font size='2'>Here, you can also find your robot status and see information like the battery level, localisation and stance. |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Localise the robot by matching the point cloud of the current lidar scan to the map.</p></div><font size="3"><font size="2"> Use the following buttons to help you achieve a good localisation.<br>![Localize Button Options](img/localize-buttons-options.png){style="width: 400px;margin-top: 10px;"}<br>Set Initial Pose: Press on the point of the map where the robot is located and drag it to the direction it is facing.<br> Rotate Pose: Used to adjust the rotation of the robot's LiDAR scan.<br>Move Pose: Used to move the robot's LiDAR scan around the map.<br> Reset Pose: Resets your current localisation. <br> Done Button: Saves your current localisation.<br><br> To localize your robot, start by selecting the 'Set Initial Pose' button. Press on the point of the map where the robot is located and drag it to the direction it is facing. Then, use the directional arrows in 'Move Pose' to adjust the robot's LiDAR point cloud to fit the map as shown in the example below.<br> ![Localize Demo GIF](img/localize-demo.gif){style="margin-top: 10px;"}<br>Additionally, you can use 'Rotate Pose' to rotate the LiDAR point cloud to make fitting it to the map easier.<br>![Localize Rotation](img/localize_rotation.gif){style="margin-top: 10px;"}<br> Refer to the examples below for instances of successful robot localisation. You may also refer to the 'Robot Status' section where the localisation result is shown. ![Localisation Examples](img/localisation.png){style="margin-top: 10px;"}The localisation of the robot is good when the robot's current LiDAR scan (white points) is aligned well to the map, meaning it has a good initial pose estimate. The localisation on the other two examples are bad as the LiDAR scan does not line up with the map, and the robot is in the wrong position.  |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Bring down the plane of the map.</p></div><font size="3"><font size="2"> Using the slider on the left, adjust the map plane such that the floor of the map is now visible. |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Once you are done with setting your robot's initial pose estimate, select the 'Done' button.</p></div><font size="3"><font size="2"> On the other hand, if you would like to restart the localisation process, press on the 'Reset Pose' button. |

Upon submitting the initial pose estimate, the robot will attempt to determine its current position on the map. During this process, there may be a momentary "jump" in the robot's position. You are advised to wait for a few seconds to ensure that the robot stabilises and remains at the correct position. Alternatively, you can manually move the robot around using the robot's controller to ensure that the LiDAR point cloud is still aligned with the map. 

Redo the localisation process if the LiDAR point cloud no longer aligns with your map. 

---

<div id="section6"></div>

### 6. Plan Tab
The plan tab is used for preparing routes for your robots to follow and perform BLK scans.
![Plan Tab View](img/plan-tab.png){style="margin-top: 10px; width: 1000px;"}

<div id="section6_1"></div>

#### 6.1 Creating your route
Before starting, ensure that you have our localised your robot to the map. Refer to [Section 5.3](#section5_3) if you require a guide to localise your robot onto the map. 

At the bottom right corner of your screen, select on the 'Add Route' button.<br>    
![Add Route Button](img/add-route-button.jpg){style="width: 300px; margin-top: 10px'"}

Give your new route a name. It is advised to use a name that is descriptive and well labelled.<br>
![Add New Route](img/add-new-route.jpg){style="width: 300px; margin-top: 10px;"}

<div id="section6_1_1"></div>

#### 6.1.1 Create routes by manually controlling of your robot
From the list of routes on the right side, select the route that you have just created and press the 'Record Route' button boxed in red to record your route. 
![Record Route Button](img/record-route-button.png){style="margin-top: 10px; width: 1000px;"}

You will then be directed to the route recording view. Here, you will be able to use the joysticks and 'Add Point' buttons at the bottom to manually control your robot, creating your route. 
You are advised to use a smaller recording interval (1 metre or smaller) when making turns. <br>
![Record Route View GIF](img/record-route-view.gif){style="margin-top: 10px;"}

After moving your robot, you should see a blue-coloured path being formed by the robot. This is the path your robots will follow when you run the route you are creating.

Once you are finished with setting your route, press 'Save Recorded Route' at the bottom of the screen and you will be directed back to the routes page with your new route saved. Now, you will be able to make your robot run the route you have created. Refer to [Section 6.3](#section6_3).

<div id="section6_1_2"></div>

#### 6.1.2 Create routes by plotting waypoints on the map
From the list of routes on the right side, select the route that you have just created and press this button boxed in red to record your route. <br>
![Edit Waypoint Button](img/edit-waypoint-route-button.png){style="width: 1000px; margin-top: 10px;"}<br>
You will then be directed to the waypoint editing page.<br>
![Set Route Page View](img/set-route-view.jpg){style="width: 1000px;"}<br>
Here, you will be able to use the buttons below to add, delete and move waypoints around the map to create the final route for your robot to follow. <br>
![Set Route Buttons](img/set-route-buttons.png){style="width: 300px; margin-top: 10px;"}

Add Mode: Add waypoints by manually plotting them onto your map<br>
Remove Mode: Remove waypoints by selecting the waypoint you want to remove on the map<br>
Move Mode: Move waypoints from one point of the map to another<br>
Done Button: Finalise and save your plotted route. <br>
Scan Mode: Covered in [Section 6.1.3.3](#section6_1_3_3).


To plot your route, select the 'Add Mode' button at the bottom of the screen. Then, plot the various points on the map where you want your robot to travel along. Ensure that the points are next to each other, avoiding any obstacles in the map and hence in real life.<br>
![Setting Route By Waypoint GIF](img/setting-route-by-waypoint.gif){style="width: 400px; margin-top: 10px;"}

If you want to delete a waypoint, select the 'Remove Mode' button, and click on the waypoints that you would like to delete.

If you would like to move one of your waypoints, select the 'Move Mode' button and press on the waypoint that you would like to move. Drag this waypoint to your desired location on the map. 

Once you are finished with plotting your route, select the 'Done' button on the left of the mode buttons. Now, you will be able to make your robot run the route you have created. Refer to [Section 6.3](#section6_3).

<div id="section6_1_3"></div>

#### 6.1.3 BLK Scanning
Before setting BLK scan points, you can configure your LiDAR configurations depending on your use case. 
![BLK Scan View](img/blk-scan-view.png){style="width: 1000px; margin-top: 10px;"}

<div id="section6_1_3_1"></div>

#### 6.1.3.1 BLK Configurations
##### LiDAR Scan Quality

LiDAR Scan Quality affects the rotation speed of the LiDAR, with "Low" indicating a slower rate and "High" representing a faster rate. Adjusting this setting directly impacts the density of data points generated in your point cloud map.

![LiDAR Scan Quality Options](img/lidar-scan-quality-options.jpg){style="width: 200px;"}

![Functionality Icon](img/pointer.png){ style="height:20px;" } Low: This option would produce a sparse point cloud map, but it does so at a much quicker rate.

![Functionality Icon](img/pointer.png){ style="height:20px;" } Medium: This option strikes a balance between point cloud density and scanning efficiency.

![Functionality Icon](img/pointer.png){ style="height:20px;" } High: This option will generate a dense point cloud map, but it takes considerably more time to do so.

##### Image Capture Mode

![Image Capture Mode Options](img/image-capture-mode-options.jpg){style="width: 200px;"}

![Functionality Icon](img/pointer.png){ style="height:20px;" } None: Does not utilize the camera for capturing images.

![Functionality Icon](img/pointer.png){ style="height:20px;" } LDR (Low Dynamic Range): Details in shadows may be lost or details in highlights may be blown out.

![Functionality Icon](img/pointer.png){ style="height:20px;" } HDR (High Dynamic Range): More detail in both highlights and shadows can be captured. 

<div id="section6_1_3_2"></div>

#### 6.1.3.2 Auto generation of scan points
In this section, you can automatically generate BLK scanning points in your route based on the distance travelled by the robot.
To use this, you must already have a route with waypoints. If you do not have one, refer to [Section 6.1.1](#section6_1_1) for a guide on recording your waypoints by manually controlling your robot or refer to [Section 6.1.2](#section6_1_2) for a guide on creating your route by manually plotting waypoints.

To enable this feature, turn this option on and set a distance interval. If your set distance interval is two metres, the robot will run a BLK scan roughly every two metres travelled along your route.
![Auto Generate Scan Points GIF](img/auto-generate-scan-points.gif){style="margin-top: 10px;"style="margin-top: 10px;"}
The generated blinking points on the map is where your robot will apply a BLK scan.<br>
To clear all BLK scanning points, select 'Clear all Scan Points' in the options menu. 

<div id="section6_1_3_3"></div>

#### 6.1.3.3 Manually setting scan points
To use this, you must already have a route with waypoints. If you do not have one, refer to [Section 6.1.1](#section6_1_1) for a guide on recording your waypoints by manually controlling your robot or refer to [Section 6.1.2](#section6_1_2) for a guide on creating your route by manually plotting waypoints.
Select the Scan Mode button at the bottom of the screen, and press the waypoints where you want your robot to perform a BLK scan. 
![Manual Select Scan Points GIF](img/manual-select-scan-points.gif){style="margin-top: 10px;"}

<div id="section6_2"></div>

#### 6.2 Editing or deleting your routes
Navigate to the right-hand side, where you'll find a list of the routes you've created. To edit or delete any of these routes, press and hold on the desired route. This action will reveal options such as rename, copy, and delete at the bottom of the screen.
![Edit Route GIF](img/edit-route.gif){style="margin-top: 10px;"}

<div id="section6_3"></div>

#### 6.3 Running your routes
| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Select the route that you would like to run.</p></div><fonst size="3"><font size='2'>You can find your routes in the routes section of the 'Plan' tab.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Once select, press the 'Set Route' button located at the bottom of the screen.</p></div><font size="3"><font size="2">![Run Route View](img/run-route-view.png){style="margin-top: 10px; width: 1000px;"}|
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Switch to the 'Ready' tab and change the control mode to 'Auto'.</p></div><fonst size="3">![Ready Tab Auto Toggle](img/running-route-ready-tab.png){style="width: 1000px; margin-top: 10px;"}|
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Your robot will now run and follow the route that you've created.</p></div><fonst size="3"><font size='2'>|

<div id="section7"></div>

#### 7. Offline Mode
If your scanning location does not have internet access, you can connect to your robot's hotspot through your device's Wi-Fi settings and use offline mode to login to your robot to carry out the same tasks as you would in online mode. To use this, you may follow the instructions below. 

Before using offline mode, ensure that your map has already been downloaded in online mode. This is because there is no internet connection and the app is unable to fetch the maps from your cloud.  Refer to [Section 3.2](#section3_2) for a guide on loading your map into the application. 
 
| Instructions |
| ------- | 
| <div class="instructions-div" id="step1"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Set a local password to enable local robot login</p></div><fonst size="3"><font size='2'>Logged into the application (online mode), head into the 'Ready' tab and select 'Set Local Password' on the right of the screen.<br>![Set Local Password](img/set-local-password.jpg){style="width: 300px; margin-top: 10px;"}<br>For security purposes, you are advised to use a strong password that you can remember to prevent unauthorised access to your robot.<br>![Local Password Prompt](img/local-password-prompt.jpg){style="width: 300px; margin-top: 10px;"} |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Connect to your robot's Wi-Fi hotspot.</p></div><fonst size="3"><font size='2'>Navigate into your device's settings, connections -> Wi-Fi, and connect to your robot's hotspot network. <br> ![Connected To Robot WiFi](img/connected-to-robot-wifi.jpg){style="width: 600px; margin-top: 10px;"}<br>Your robot's Wi-Fi network name and password will be provided to you. If you have trouble connecting to your robot's network, please contact us for support. |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Head back into the application and enter offline mode that can be found in the login page.</p></div><fonst size="3"><font size='2'>![Offline Mode Button](img/offline-mode-button.png){style="width: 600px; margin-top: 10px;"}<br>|
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Connect to your robot.</p></div><fonst size="3"><font size='2'>On the left hand side of the main page, select on this button boxed in red to connect to your robot.<br>![Select Robot](img/select-robot.png){style="width: 300px; margin-top: 10px;"}<br>Your robot should appear now in the form of its IP address.<br>![Offline Mode Connect To Robot](img/offline-mode-connect-to-robot.jpg){style="width: 600px; margin-top: 10px;"}<br>Select your robot and enter the local password that you have previously set in [Step 1](#step1) to finally login.|

You are now using offline mode. Now, you will be able to access the application's functionalities in locations without internet access.

---

That is all for d.ASH Nav!
If you require any support, please feel free to contact us [here](mailto:hello@dconstruct.co) if you encounter any difficulties.

This document was last updated on: 9 October 2023
