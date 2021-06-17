# dConstruct d.ASH SDK

The [dConstruct d.ASH SDK](https://www.dconstruct.co/services-1) a cross-platform library for autonomous robot navigation. Use the d.ASH SDK to develop applications for your own [Spot](https://www.bostondynamics.com/spot) from Boston Dynamics or any other robot you wish. This section of the d.ASH SDK documentation provides details about the components of the SDK.

![Screenshot](img/diagram.png){: .center style="width:550px" }

| Component | Description |
| ------- | ------- |
|  **[d.ASH Server](https://dconstruct-tech.github.io/dash-sdk/#dash-server)** | <font size="3"> The d.ASH server acts as the main server responsible for sending control commands to the robot. At the same time, the d.ASH server also broadcasts secured data to any given remote systems.|
|  **[d.ASH Autonomy Engine](https://dconstruct-tech.github.io/dash-sdk/#ros-driver)** | <font size="3"> The d.ASH Autonomy Engine is the autonomy backend code that runs on the edge of the robot. It empowers the robot with robust multi-terrain (indoor and outdoor) autonomous navigation capabilities. It handles secure communication between automony engine and the remote autonomy controller. |
| **[d.ASH Autonomy Controller](https://dconstruct-tech.github.io/dash-sdk/#dash-autonomy-controller)** | <font size="3"> The d.ASH autonomy controller is the GUI (graphical user interface) for the d.ASH autonomy engine. It enable users to monitor and have full remote control of autonomy by allowing users to plot waypoints and activate autonomy on a fleet of robots. Stream real-time data via a secure connection between robots and the controller using 4G or 5G. |


If you decide to use your own custom GUI in place of the [d.ASH Autonomy Controller](#dash-autonomy-controller), or you do not want to run autonomy, you will still need to implement the [d.ASH Server](#dash-server) and the [ROS Driver](#ros-driver) to operate your robot. 
