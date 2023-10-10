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

# d.ASH Go

### Introduction 

Welcome to the d.ASH Go application user guide! This comprehensive guide will walk you through the process of installing the application and providing the necessary instructions for your map scanning process. To access the user guide for our application, please refer to [Section 2](#section2) in this page. Otherwise, if you would like to scan maps on your web browser, please turn to [Section 3](#section3).
![d.ASH Go](img/d.ASHGo/dash-go.png){margin-top="-20"; width="1200"}

### Application Functions 
d.ASH Go is our visualisation system that allows you to see where you've mapped on the fly in just two easy steps! The point clouds are generated in real time, giving you a preview of what the final generated map would look like. 

Before starting, an internet connection from your d.ASH Pack is required. If you are having trouble connecting to your d.ASH Pack's network, please contact us [here](mailto:hello@dconstruct.group) for more information.


![Functionality Icon](img\d.ASHGo\pointer.png){style="height:20px;"} Real-time mapping visualisation

Joins spatial data on the fly, allowing users to generate long expressions in order to visualize the data of their surrounding environment. This can be used for transferring environmental data to autonomous robots for them to traverse through the environment.

### d.ASH Go Android Application
Before installing the application, ensure that your mobile device meets the minimum system requirements. 

#### System Requirements

| Minimum System Requirements                                       | Recommended System Requirements                                   |
|-------------------------------------------------------------------|-------------------------------------------------------------------|
| Android Tablet with support for OpenGL ES 3.2                     | Android Tablet with support for OpenGL ES 3.2                     |
| Operating System: Android Version 13 \| Tiramisu \| API Level 33  | Operating System: Android Version 13 \| Tiramisu \| API Level 33  |
| CPU: Qualcomm Snapdragon 720G                                     | CPU: Snapdragon 888 Chip                                          |
| GPU: Adreno 618                                                   | GPU: Adreno 730                                                   |
| RAM: 4 GB                                                         | RAM: 8 GB                                                         |

#### Installation Guide

Click [here](https://play.google.com/store/apps/details?id=ai.dconstruct.dashpack) to install the d.ASH Go application on your Android device. Alternatively, you can enter the Google Play Store and search for our app. 

![Google Play App Search](img\google-play.png){style="width: 600px;"}

#### Quick Start Guide
The following section provides a step-by-step guide to help you start recording with your d.ASH Pack. Additional features offered by d.ASH Go are listed in the subsequent sections.


| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;"> Open your mobile device's settings app, click on Connections -> Wi-Fi, and then connect to the network of your d.ASH Pack. </p></div><font size="2"> You can find the name and password of the network on your d.ASH Pack's hatch. After a successful connection, there should be a message saying 'Connected without internet' at the bottom of the network. <br> ![d.ASHpack Hatch](img/d.ASHGo/dashpack-hatch.png){style="width: 500px"}<br> When a connection has been established, your device may prompt for action as internet will not be available on the network, choose **Always Connect** for the device to work properly with d.ASH Pack.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Open the application, ensure that all icons under d.ASH Pack Status are green in colour.</p></div><font size="2"> All icons must be green and ready to start before starting a new map scan.<br>![d.ASHpack Status](img\d.ASHGo\dashpack-status.png){style="width: 500px;margin-top: 10px"}<br> If the Wi-Fi icon is red, please check your network connection and ensure that you are connected to your d.ASH Pack. If you encounter any issues, please feel free to contact us [here](mailto:hello@dconstruct.group). |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Press start a new scan and check the appropriate checkboxes for the type of scan you wish to perform. Press start. </p></div><font size="2"> You are advised to give your scans descriptive and memorable names. <br>![Scan Settings](img\d.ASHGo\scan-settings.jpg){style="width: 500px; margin-top: 10px"}<br> It is recommended to set your d.ASH Pack to have an upright sensor when you want non-coloured scans.<br> On the other hand, having a slanted sensor is recommended for coloured scans. |
| <div class="instructions-div" id="headers"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Press the start button at the bottom when you are ready to start scanning. </p></div><font size="2"> <strong>Before you start, here are some headers to take note of while scanning your location: </strong><br>1. It is not possible to pause and continue a scan in the app. Scanning must be completed in one continuous session. <br>2. For the best results, avoid taking sharp and suddden turns when turning corners; take slow and gradual ones instead.<br>![Correct Turn Example](img/d.ASHGo/correct-turn.png){style="width: 800px; margin-top: 10px"}<br>3. Move at a steady pace.<br>4. If any of the icons turn red during the scan, you will need to restart from the beginning and make sure that you are connected properly to your d.ASH Pack. If the same issue persists, please contact us for support. ![Play Button](img\d.ASHGo\play-button.png){style="width: 800px;margin-top: 10px"} <br>Only begin scanning when you are in the desired location.</br> |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Start scanning! </p></div><font size="2">The scan status icon on the top right corner of the application and the LED on your d.ASH Pack will turn yellow. While following the previously mentioned [headers](#headers), walk around your location until you have covered the majority of it and, if possible, return to where you started.<br>![Live Scan GIF](img/d.ASHGo/live-scan.gif){style="width: 800px;margin-top: 10px"}<br>Swipe with one finger to rotate view, swipe with two fingers to move around the map. Pinch in and out to change the zoom. |
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;">Press and hold on the stop button to finish the map scan. </p></div><font size="2"> Well done! Now, you can preview your scan by selecting on your scan on the home page and pressing open scan at the bottom right. |

If there are major misalignments present in your scan, it is recommended to perform the scan once again. If not, you are good to go!
Use your map scan for further preprocessing in [d.ASH Xplorer](https://dconstruct-tech.github.io/dash-sdk/dash-pack/dash-xplorer/#251-point-cloud-editor) or upload it into the [d.ASH Nav](https://dconstruct-tech.github.io/dash-sdk/dash-auto/autonomy-client-v2/) application for use in robot automation.

Last updated: 10/10/2023