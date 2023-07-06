<!--
1. Login process
    1.1: DL from fleet management
    1.2: Login with credentials we generate for you
    1.3: If there's trouble logging in. Email/call dC

2. Project browser
    2.1: Create new project
    2.2: Opening existing project
    2.3: Map browser/open map

3. Main menu
    3.1: Explain each tab on the top bar (left to right)
    3.2: Explain main dash nav screen n sliders etc
    3.3: Explain side bars (top to bottom)
        3.3.1: Routes container (All routes saved by user, when expanded can see which robo is assigned to it. Can also add or remove robots from selected route)
        3.3.2: Robot list (Shows all currently connected robots only)
        3.3.3: Visualisation (Yang Kai's colour blind solver and other visual edits like scale of objects)

4. Plan tab
    4.1: Actions
        4.1.1: Explain autodrive
        4.1.2: How to record waypoint
        4.1.3: Create route
    4.2: Waypoint Editing
        4.2.1: Edit waypoint (add, delete, reposition)
        4.2.2: Interpolate (Auto waypoint recording)
        4.2.3: Set scan points (Set selected/all/delete, for BLK etc)
    4.3: Connect to :b:obots

5. Ready tab
    5.1: Estop/resume
    5.2: List of robots (Loads popup)
        5.2.1: Checklist/health monitor
        5.2.2: Robot info
        5.2.3: Control panel/robot settings
    5.3: Robot actions
        5.3.1: Localise
        5.3.2: Follow cam
        5.3.3: Auto/Manual control
        5.3.4: Sit/Stand spot only
    5.4: Assign route to robot
        5.4.1: Drop down
        5.4.2: Tag robot

6. Monitor tab
    6.1: Estop/resume
    6.2: Live views (Cams can be frm any mix of robots)
        6.2.1: Mapview (Smol view of robo cams)
        6.2.2: 4 view (4 cams n no map)
        6.2.3: Focus (Focus on one cam, no map)
    6.3: Robo Controls
        6.3.1: Run route given to robot
        6.3.2: Autodrive
        6.3.3: Auto/Manual Sit/Stand

-->

# **1. d.ASH Nav**
*d.ASH Nav* is *the* platform for autonomous control of robots. Being seamlessly integrated in the [d.ASH Fleet Management](https://www.dconstruct.co/products) workflow, you can enjoy easy planning and deployment of your robots for various use cases. *d.ASH Nav* allows you to plot waypoints for autonomous navigation on maps, tracking and monitoring path planning, as well as overall monitoring of your robots.

Because *d.ASH Nav* is fully integrated with [d.ASH Fleet Management system](https://www.dconstruct.co/products), an internet connection is required. Should you require *d.ASH Nav* without an internet connection, please [contact us](mailto:hello@dconstruct.ai) for more details.

### **1.1 Minimum System Requirements**

1. PC with a CPU equivalent to or greater than an Intel i5 4th Gen or AMD R5 1000 series
2. Nvidia GTX 960
3. 8GB of RAM
4. Internet Connection
5. Windows 10/11
6. Gamepad/Joystick (e.g. Logitech F710 Gamepad)

*We recommend using a discrete Nvidia GPU greater than or equivalent to an RTX 3060. Some features may run slower on other GPUs. A joystick is recommended for manual tele-operation control.*

### **1.2 Tutorial**

**Control Scheme**

*d.ASH Nav*'s control scheme is as follows:

- Tilt/Camera: Hold down the *Left Mouse* Button and drag
- Zoom: Use the mouse scroll wheel to zoom in/zoom out
- Move Around: Use the *WASD* keys to pan/move around the world

### **1.3 Quick Start**

The general workflow to operate and run an autonomous waypoint mission is as follows:

1. Login to *d.ASH Nav*
2. Create a new project, this allows you to save any routes created for use later on
3. Load the map of your choice
4. Create a new mission Route and plot the waypoints
5. Connect to your desired robot in your robot fleet
6. Set the robot's initial starting pose on the 3D map
7. Start the robot with the route for your new mission

## **2. Login process**

### **2.1 Fleet Manager**
First, login to Fleet Manager with your given credentials to download the latest build of *d.ASH Nav*.
Next, login to d.ASH Nav.
If you encounter any difficulties logging in, please [contact us](mailto:hello@dconstruct.ai).

## **3. Project management**
Once you've logged in, you will be greeted by the project window. Here, you can manage all existing projects as well as create new projects. These projects are synced to the cloud, thus allowing you to manage your projects and use *d.ASH Nav* from anywhere in the world!

### **3.1 Creating a project**
To create a new project, simply click on the "New Project" button. You will then be prompted to enter a project name. After creating your new project, you will be redirected to the *Map Browser*.  If a project with the same name exists, a prompt will pop up asking you to choose another name for the project.

### **3.2 Loading an existing project**
To load an existing project, select an existing project saved to the cloud using the file browser on the right hand side of the screen. Alternatively, if you are loading a project saved locally, click on the "Browse" button and navigate to the local location of the project. After creating your new project, you will be redirected to the *Map Browser*.

### **3.3 Map Browser**
After creating/loading an existing a project, you will be taken to the *Map Selection Screen*. This screen allows you to select the map which relates to your deployment location. After selecting your map, you can begin to deploy your robots. Maps can be sorted by whether they are coloured or not.

## **4. Main Menu**
This is the main hub of all things *d.ASH Nav*. Everything concerning deployment of your robots can be found here.

## **4.1 Top Menu**
The top bar contains several crucial pieces of information, such as which part of the deployment process you are currently in and actions that you can perform in each part of deployment. In the *Main Menu*, options to manage your projects and browse through available maps are available. The arrows indicate the proper flow of how a deployment should be run.

### **4.1.1 Project Options**
- *New Project*: Create a brand new project
- *Open Project*: Load an existing project
- *Save*: Save any changes to the current project
- *Save as*: Save any changes to the current project under a different file/project name
- *Preferences*: Edit *d.ASH Nav* settings

### **4.1.2 Map Browser**
- *Map Browser*: Browse through all maps saved to your account

## **4.2 View Port**
This is a visual representation of the map you have loaded for your project. 

- *View Toggles*: A widget in the top left corner of the *View Port* which allows you to toggle the visiblity of certain objects in the *View Port*.
- *Orientation Gizmo*: A gizmo in the top right corner of the *View Port* shows the current orientation of the map, relative to the orientation of the floor.
- *Height Sliders*: Adjust the cut off points for rendering of the loaded map.

## **4.3 Side Bar**
The *Side Bar* contains all information to do with any planned routes, connected robots and *View Port* visualisation tweaks

- *Routes*: Contains all planned routes in the project with the ability to toggle the preview of the route in the *View Port*, view all robots assigned to this route, assign new robots to this route and delete existing routes. This also reflects the current mission's route and status.
- *Robot List*: Shows you all currently connected robots and their status.
- *Visualisation*: Allows for you to tweak the colour of elements in the rendered point cloud as well as the scale (size) of the rendered robot and waypoints. This is more useful for those who experience colour blindness. We recommend leaving these settings at their default value.

## **5. Plan Tab**
This tab contains all actions to do with planning routes.

### **5.1 Actions**
Three actions are available for you to use:

- *Autodrive*: Using machine learning and computer vision to analyze and understand your robot's surroundings, hands-free Level 2 Autonomy allows for the navigation of complex, unstructured environments using just cameras alone.
- *Record Waypoints*: Records and plots waypoints as you manually navigate the robot in real life.
- *Create Route*: Creates an empty route for you to edit and add waypoints later on.

### **5.2 Waypoint**
This menu contains all available actions for editing waypoints on a route. This is greyed out by default and will only be accessible after selecting a route to edit. Several options are available to you.

- *Edit Waypoint*: Enters a seperate mode containing actions to edit waypoints in a selected route
- *Interpolation by distance*: Adds additional waypoints between two existing waypoints which are too far apart. This allows for more actions (such as scans) to be excuted along a given path. The default interval is set at 1m.
- *Set scan points*: The robot will stop to perform a scan with 3rd party scanners.

### **5.3 Schedule**
This menu allows you to set a start date and time for your robots to automatically execute pre-planned missions.

### **5.4 Robots**
Clicking this button will show a popup containing a list of all available robots. Connect to your preferred robot from this popup menu.

## **6. Ready Tab**
This tab contains all actions necessary to deploy your robot

### **6.1 E-Stop/Resume**
Controls for stopping and resuming a mission/robot movement can be found here.

### **6.2 List of robots**
Shows a list of all connected robots with several different pieces of information tied to each robot.
- *Health Monitor*: The health monitor shows the status of all sensors on the robot.
- *Robot Info*: Contains info such as the robot's serial number, date of purchase etc
- *Robot Settings*: Adjust the tag settings of a selected robot through colour tags.

### **6.3 Robot Actions**
- *Localise*: Give the robot an estimate of where it currently is on the map in order for the robot to fine tune its position.
- *Follow Cam*: Sets the camera of the *View Port* to follow and track the robot as it moves throughout the map.
- *Auto/Manual Control*: Manually change the operating mode of the selected robot.
- *Sit/Stand Robot*: **SPOT ONLY**. Sit or stand Boston Dynamics Spot Robot.

### **6.4 Assign Route to Robot**
- *Drop Down*: Choose the route to assign.
- *Tag Robot*: Choose the robot to assign the route to (i.e: tagging the robot)

## **7. Monitor Tab**
This tab contains all actions and information about the mission in progress.

### **7.1 E-Stop/Resume**
Controls for stopping and resuming a mission/robot movement can be found here.

### **7.2 Live views**
Views from the cameras on the robots can be found here. To add a view, simply drag and drop a robot from the right side bar into an empty view slot and select which camera to view. There are three templates to follow.

- *Map View*: Shows less of the view from the robot cameras to make space for viewing the Point Cloud Map.
- *Four View*: This view will completely hide the Point Cloud Map and instead show four slots for different robot camera views.
- *Focus*: This view will completely hide the Point Cloud Map and instead show only one robot camera view.

### **7.3 Robot Controls**
- *Run Route*: Issues the command to the selected robot to run its assigned route
- *Autodrive*: [See above](#51-actions)
- *Auto/Manual | Sit/Stand*: [See above](#63-robot-actions)