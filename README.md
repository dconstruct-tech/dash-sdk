<p align="center"><img src="docs/img/dASH-logo.jpg" width="25%" /><br><br></p>

-----------------

## Overview
**dConstruct d.ASH SDK** is a cross-platform library for autonomous robot navigation. Use the d.ASH SDK to develop applications for your own Spot from Boston Dynamics or any other robot you wish. 

> :pushpin: For more information on the d.ASH SDK documentation, please refer to the [latest documentation release](https://dconstruct-tech.github.io/dash-sdk/).

## What’s included in the SDK:
| What | Description |
| ------- | ------- |
| **[d.ASH Server](https://dconstruct-tech.github.io/dash-sdk/#dash-server)** | The d.ASH server acts as the main server responsible for sending control commands to the robot. At the same time, the d.ASH server also broadcasts secured data to any given remote systems.|
| **[d.ASH Autonomy Engine](https://dconstruct-tech.github.io/dash-sdk/#ros-driver)** | The d.ASH Autonomy Engine is the autonomy backend code that runs on the edge of the robot. It empowers the robot with robust multi-terrain (indoor and outdoor) autonomous navigation capabilities. It handles secure communication between automony engine and the remote autonomy controller. |
| **[d.ASH Autonomy Controller](https://dconstruct-tech.github.io/dash-sdk/#dash-autonomy-controller)** | The d.ASH autonomy controller is the GUI (graphical user interface) for the d.ASH autonomy engine. It enable users to monitor and have full remote control of autonomy by allowing users to plot waypoints and activate autonomy on a fleet of robots. Stream real-time data via a secure connection between robots and the controller using 4G or 5G. |

## License
This project is licensed under the [BSD 2-Clause License](LICENSE).
Copyright 2021 dConstruct Technologies Pte Ltd.

To find out more about dConstruct Technologies [now](https://www.dconstruct.co/).
