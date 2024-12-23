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

    .instructions-div p {
        font-size: 18px;
    }
</style>

# **1. d.ASH Ops**
*d.ASH Ops* is *the* platform for autonomous control of robots. Being seamlessly integrated in the [d.ASH Fleet Management](https://www.dconstruct.co/products) workflow, you can enjoy easy planning and deployment of your robots for various use cases. *d.ASH Ops* allows you to plot waypoints for autonomous navigation on maps, tracking and monitoring path planning, as well as overall monitoring of your robots.

Because *d.ASH Ops* is fully integrated with [d.ASH Fleet Management system](https://www.dconstruct.co/products), an internet connection is required. Should you require *d.ASH Ops* without an internet connection, please [contact us](mailto:hello@dconstruct.group) for more details.

### **1.1 Minimum System Requirements**

1. PC with a CPU equivalent to or greater than an Intel(R) Core(TM) i5-10210U
2. Nvidia GTX 1060
3. 8GB of RAM
4. Internet Connection
5. Windows 10/11
6. Gamepad/Joystick (e.g. Logitech F710 Gamepad)

*We recommend using a discrete Nvidia GPU greater than or equivalent to an RTX 3060. Some features may run slower on other GPUs. A joystick is recommended for manual tele-operation control. We also recommend 16GB of RAM for smoother operation*

### **1.2 Tutorial**

**Control Scheme**

*d.ASH Ops*'s control scheme is as follows:

- Tilt/Camera: Hold down the *Right Mouse* Button and drag
- Zoom: Use the mouse scroll wheel to zoom in/zoom out
- Move Around: Use the *WASD* keys to pan/move around the world

### **1.3 Quick Start**

The general workflow to operate and run an autonomous waypoint mission is as follows:

| Instructions |
| ------- | 
| <div class="instructions-div" id="step1"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Login to *d.ASH Ops* with your given credentials.</p></div><img alt="Login Screen" src="img/dash-ops/login-screen.png" width="600px"> |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Create a new project.</p></div><font size='2'>This allows you to save any routes created for use later on.<br><img alt="Create New Project" src="img/dash-ops/new-project.png" width="600px"> |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Load the map of your choice.</p></div><img alt="Loading Map" src="img/dash-ops/loading-map.png" width="600px"> |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Create a new mission route and plot the waypoints.</p></div><font size='2'>Refer to [Section 6](#6-plan-tab) for more details regarding creating a route.<br> |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Connect to your desired robot in your robot fleet.</p></div><img alt="Connecting To Robot" src="img/dash-ops/connecting-robot.png" width="600px"> |
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;">Set the robot's initial starting pose on the 3D map.</p></div><font size='2'>Refer to [Section 7.3.1](#731-localisation) for more details on how to localise your robot.<br><img alt="Relocalising Robot" src="img/dash-ops/set-initial-pose.png" width="600px"> |
| <div class="instructions-div"><div class="instruction-circle">7</div><p style="margin: 0; margin-left: 5px;">Start the robot with the route for your new mission.</p></div> |

## **2. Download**
Please [contact us](mailto:hello@dconstruct.ai) for the link to download *d.ASH Ops*.

## **3. Project Management**
Once you've logged in, you will be greeted by the project window. Here, you can manage all existing projects as well as create new projects. These projects are synced to the cloud, thus allowing you to manage your projects and use *d.ASH Ops* from anywhere in the world!
<img alt="Project Management" src="img/dash-ops/open-folder.png" width="600px">

### **3.1 Creating a project**
To create a new project, simply click on the "New Project" button. You will then be prompted to enter a project name. After creating your new project, you will be redirected to the *Map Browser*.  If a project with the same name exists, a prompt will pop up asking you to choose another name for the project.

### **3.2 Loading an existing project**
To load an existing project, select an existing project saved to the cloud using the file browser on the right hand side of the screen. Alternatively, if you are loading a project saved locally, click on the "Browse" button and navigate to the local location of the project. After creating your new project, you will be redirected to the *Map Browser*.

### **3.3 Map Browser**
After creating/loading an existing a project, you will be taken to the *Map Selection Screen*. This screen allows you to select the map which relates to your deployment location. After selecting your map, you can begin to deploy your robots. Maps can be sorted by whether they are coloured or not.
<img alt="Loading Map" src="img/dash-ops/loading-map.png" width="600px">

## **4. Navigating d.ASH Ops**
This section will list the different elements of the user interface of *d.ASH Ops*.

### **4.1 Top Menu**
<img alt="Top Menu" src="img/dash-ops/top-menu.png" width="600px"><br>
The top bar contains several crucial pieces of information, such as which part of the deployment process you are currently in and the actions that you can perform in each part of deployment. The arrows indiate the proper flow of how a deployment should be run.

### **4.2 View Port**
<img alt="View Port" src="img/dash-ops/view-port.png" width="600px"><br>
This is a visual representation of the map you have loaded for your project. 

- *View Toggles*: A widget in the top left corner of the *View Port* which allows you to toggle the visiblity of certain objects in the *View Port*.
- *Height Sliders*: Adjust the cut off points for rendering of the loaded map.
<!-- - *Orientation Gizmo*: A gizmo in the top right corner of the *View Port* shows the current orientation of the map, relative to the orientation of the floor. -->

### **4.3 Side Bar**
The *Side Bar* contains all information to do with any planned routes, connected robots and *View Port* visualisation tweaks.<br>
<img alt="Side Bar" src="img/dash-ops/side-bar.png" width="600px"><br>
- *Routes*: Contains all planned routes in the project with the ability to toggle the preview of the route in the *View Port*, view all robots assigned to this route, assign new robots to this route and delete existing routes. This also reflects the current mission's route and status.
- *Robot List*: Shows you all currently connected robots and their status.
- *Visualisation*: Allows for you to tweak the colour of elements in the rendered point cloud as well as the scale (size) of the rendered robot and waypoints. This is more useful for those who experience colour blindness. We recommend leaving these settings at their default value.

## **5. Main Menu**
This is the main hub of all things *d.ASH Ops*. Everything concerning deployment of your robots can be found here.

### **5.1 Project Options**
- ![Screenshot](img/icons/NewProject_32_Black.png) *New Project*: Create a brand new project
- ![Screenshot](img/icons/OpenProj_32_Black.png) *Open Project*: Load an existing project
- ![Screenshot](img/icons/Save_32_Black.png) *Save*: Save any changes to the current project
- ![Screenshot](img/icons/SaveAs_32_Black.png) *Save as*: Save any changes to the current project under a different file/project name
- ![Screenshot](img/icons/Prefs_32_Black.png) *Preferences*: Edit *d.ASH Ops* settings

### **5.2 Map Browser**
- ![Screenshot](img/icons/MapBrowser_32_Black.png) *Map Browser*: Browse through all maps saved to your account


## **6. Plan Tab**
This tab contains all actions to do with planning routes.

### **6.1 Actions**
Three actions are available for you to use:

- ![Screenshot](img/icons/Autodrive_32_Black.png) *Autodrive*: Using machine learning and computer vision to analyze and understand your robot's surroundings, hands-free Level 2 Autonomy allows for the navigation of complex, unstructured environments using just cameras alone.
- ![Screenshot](img/icons/WPRec_32_Black.png) *Record Waypoints*: Records and plots waypoints as you manually navigate the robot in real life.
- ![Screenshot](img/icons/AddRoute_32_Black.png) *Create Route*: Creates an empty route for you to edit and add waypoints later on.

### **6.2 Edit Waypoint**
This menu contains all available actions for editing waypoints on a route. This is greyed out by default and will only be accessible after selecting a route to edit. Several options are available to you.

<img alt="Edit Waypoint" src="img/dash-ops/edit-route-menu.png" width="600px">

- ![Screenshot](img/icons/WPAdd_32_Black.png) / ![Screenshot](img/icons/WPDel_32_Black.png) *Add/Delete Waypoint*: Add or remove a waypoint from a selected route
- ![Screenshot](img/icons/WPRepos_32_Black.png) *Reposition Waypoint*: Select a waypoint to shift the waypoint from one position to another. 
- *Interpolation by distance*: Adds additional waypoints between two existing waypoints which are too far apart. This allows for more actions (such as scans) to be excuted along a given path. The default interval is set at 1m.
- ![Screenshot](img/icons/ScanEnable_32_Black.png) / ![Screenshot](img/icons/ScanDisable_32_Black.png) *Enable/Disable Scan*: Marking a waypoint as a scan point will tell the robot to stop and perform a scan with 3rd party scanners.
- ![Screenshot](img/icons/ScanAll_32_Black.png) *Scan All*: Marks all waypoint as a scan point. This will tell the robot to stop and perform a scan with 3rd party scanners.
- ![Screenshot](img/icons/Finish_32_Black.png) *Finish*: Closes the menu.

### **6.3 Recording Waypoint**
You can use a robot in your fleet to record a mission route, which you can then assign as a mission to your robots.

| Instructions |
| ------- | 
| <div class="instructions-div" id="step1"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Click 'Record Route' and name your route.</p></div><img alt="Record Button" src="img/dash-ops/record.png" style="margin-top: 10px; width: 600px;" /> |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Select the robot which you want to record the route with.<br></p></div><img alt="Select Robot" src="img/dash-ops/select-robot.png" style="margin-top: 10px; width: 600px;" /> |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Set an appropriate interval between recorded waypoints.</p></div><font size='2'>We recommend setting a lower interval in tight areas and a higher interval in open areas. |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Click 'Start' to start recording the route.</p></div> |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Through manual teleoperation, drive your robot along the route you want to be recorded.</p></div> |
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;">When you are finished recording, click 'End'.</p></div><font size="2">Your recorded route will be saved in the route list. |

### **6.4 Robot List**
Clicking this button will show a popup containing a list of all available robots. Connect to your preferred robot from this popup menu.

## **7. Ready Tab**
The **Ready Tab** contains all the actions needed for you to ready your robot for deployment.

### **7.1 E-Stop/Resume**
The emergency stop and resume buttons allow you to force-stop all robots in your fleet in the event of an emergency.

### **7.2 List of robots**
Shows a list of all connected robots with several different pieces of information tied to each robot.
- *Health Monitor*: The health monitor shows the status of all sensors on the robot.
- *Robot Info*: Contains info such as the robot's serial number, date of purchase etc
- *Robot Settings*: Adjust the tag settings of a selected robot through colour tags.

### **7.3 Robot Actions**
- ![Screenshot](img/icons/Localise_32_Black.png) *Localise*: Give the robot an estimate of where it currently is on the map in order for the robot to fine tune its position.
- ![Screenshot](img/icons/Follow_32_Black.png) *Follow Cam*: Sets the camera of the *View Port* to follow and track the robot as it moves throughout the map.
- ![Screenshot](img/icons/Auto_32_Black.png) / ![Screenshot](img/icons/Manual_32_Black.png) *Auto/Manual Control*: Manually change the operating mode of the selected robot.
- *Sit/Stand Robot*: **SPOT ONLY**. Sit or stand Boston Dynamics Spot Robot.
- *Dock*: Dock or undock robot at docking station.

#### **7.3.1 Localisation**
Before running a mission, you should make sure that your robot is localised to ensure that it follows the route accurately.

| Instructions |
| ------- | 
| <div class="instructions-div" id="step1"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;">Select the robot that you want to localise and click 'Localise'.</p> |
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Click 'Set Initial Pose', and then click on the point of the map where the robot is located and drag it in the direction it is currently facing.</p></div><font size="2">To ensure good localisation, the point cloud of the robot's current LiDAR scan should match to the map.</font><br><img alt="Set Initial Pose" src="img/dash-ops/set-initial-pose.png" style="margin-top: 10px; width: 600px;" /><br> |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Click on 'Relocalise' to make small adjustments to the robot's position and rotation.</p></div><font size="2">When you are finished relocalising, click on 'Relocalise' again to confirm your changes.</font><br><img alt="Relocalise" src="img/dash-ops/relocalise.png" style="margin-top: 10px; width: 600px;"> |
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">After localising, click 'Finish'.</p></div><font size="2">The localisation icon beside your robot should turn green. |

### **7.4 Assign Route to Robot**
- *Drop Down*: Choose the route to assign.
- *Tag Robot*: Choose the robot to assign the route to (i.e: tagging the robot)

## **8. Monitor Tab**
This tab contains all actions and information about the mission in progress.

### **8.1 E-Stop/Resume**
Controls for stopping and resuming a mission/robot movement can be found here.
- ![Screenshot](img/icons/Localise_32_Black.png) *Stop All*: Stops all robots in case of an emergency.
- ![Screenshot](img/icons/Resume_32_Black.png) *Resume All*: Resumes all robots that are stopped.

### **8.2 Live Views**
Views from the cameras on the robots can be found here. To add a view, simply drag and drop a robot from the right side bar into an empty view slot and select which camera to view. There are three templates to follow.

- ![Screenshot](img/icons/MapView_32_Black.png) *Map View*: Shows less of the view from the robot cameras to make space for viewing the Point Cloud Map.
- ![Screenshot](img/icons/4View_32_Black.png) *Four View*: This view will completely hide the Point Cloud Map and instead show four slots for different robot camera views.
- ![Screenshot](img/icons/FullView_32_Black.png) *Focus*: This view will completely hide the Point Cloud Map and instead show only one robot camera view.
- ![Screenshot](img/icons/Localise_32_Black.png) *Hide*: Disables all cameras/shows only the Point Cloud Map

### **8.3 Robot Controls**
- ![Screenshot](img/icons/RunRoute_32_Black.png) *Run Route*: Issues the command to the selected robot to run its assigned route
- ![Screenshot](img/icons/Autodrive_32_Black.png) *Autodrive*: [See above](#61-actions)
- ![Screenshot](img/icons/Auto_32_Black.png) / ![Screenshot](img/icons/Manual_32_Black.png) *Auto/Manual 
- *Sit/Stand*: [See above](#73-robot-actions)
- *Dock*: [See above](#73-robot-actions)

## **9. Telegram Configuration**
d.ASH Ops supports status notifications of the robots in your fleet via Telegram! Add [dconstruct-bot](https://t.me/dconstruct_bot)!

### **9.1 Setup**
1. Add the Telegram bot to the Telegram chat of your choice
2. Request for a key from us [here](mailto:hello@dconstruct.ai).
3. In the Telegram chat of your choice, use the ```/register``` command followed by the key. (e.g. ```/register [insert key here]```)

### **9.2 Remove from chat**
If you would like to stop receiving notifications, use the ```/delete``` command.