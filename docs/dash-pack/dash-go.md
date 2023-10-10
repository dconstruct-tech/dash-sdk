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

Welcome to the d.ASH Go application user guide! This comprehensive guide will walk you through the process of installing the application and providing the necessary instructions for your map scanning process. To access the user guide for our application, please refer to <a href="#section2">Section 2</a> in this page. Otherwise, if you would like to scan maps on your web browser, please turn to <a href="#">Section 3</a>.
![](img/d.ASHGo/dash-go.png){margin-top="-20"; width="1200"}

### Application Functions 
d.ASH Go is our visualisation system that allows you to see where you've mapped on the fly in just two easy steps! The point clouds are generated in real time, giving you a preview of what the final generated map would look like. 

Before starting, an internet connection from your d.ASH Pack is required. If you are having trouble connecting to your d.ASH Pack's network, please contact us <a href="">here</a> for more information.


![Functionality Icon](img\d.ASHGo\pointer.png){ style="height:20px;" } Real-time mapping visualisation

Joins spatial data on the fly, allowing users to generate long expressions in order to visualize the data of their surrounding environment. This can be used for transferring environmental data to autonomous robots for them to traverse through the environment.

### d.ASH Go Android Application

#### Installation Guide
Before installing, ensure that your mobile device meets the minimum system requirements. 

Click <a href="https://play.google.com/store/apps/details?id=ai.dconstruct.dashpack">here</a> to install the d.ASH Go application on your Android device. Alternatively, you can enter the Google Play Store and search for our app. 


#### Minimum System Requirements

Android Tablet with support for OpenGL ES 3.2
Operating System: Android Version 13 | Tiramisu | API Level 33 
CPU: Qualcomm SM7125 Snapdragon 720G (8 nm)
GPU: Adreno 618
RAM: 4 GB

![Google Play App Search](img\google-play.png){style="width: 600px;"}

#### Quick Start Guide
The following section provides a step-by-step guide to help you start recording with your d.ASH Pack. Additional features offered by d.ASH Go are listed in the subsequent sections.


| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;"> Open your mobile device's settings app, click on Connections -> Wi-Fi, and then connect to the network of your d.ASH Pack. </p></div><font size="3"><font size="2"> You can find the name and password of the network on your d.ASH Pack's hatch. After a successful connection, there should be a message saying 'Connected without internet' at the bottom of the network. <br> ![](img/d.ASHGo/dashpack-hatch.png){style="width: 500px"}<br> When a connection has been established, your device may prompt for action as internet will not be available on the network, choose **Always Connect** for the device to work properly with d.ASH Pack.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;">Open the application, ensure that all icons under d.ASH Pack Status are green in colour.</p></div><font size="3"><font size="2"> All icons must be green and ready to start before starting a new map scan.<br>![](img\d.ASHGo\dashpack-status.png){style="width: 500px;margin-top: 10px"}<br> If the Wi-Fi icon is red, please check your network connection and ensure that you are connected to your d.ASH Pack. If you encounter any issues, please feel free to contact us <a href="#">here</a>. |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;">Press start a new scan and check the appropriate checkboxes for the type of scan you wish to perform. Press start. </p></div><font size="3"><font size="2"> You are advised to give your scans descriptive and memorable names. <br>![](img\d.ASHGo\scan-settings.jpg){style="width: 500px; margin-top: 10px"}<br> It is recommended to set your d.ASH Pack to have an upright sensor when you want non-coloured scans.<br> On the other hand, having a slanted sensor is recommended for coloured scans. |
| <div class="instructions-div" id="headers"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;">Press the start button at the bottom when you are ready to start scanning. </p></div><font size="3"><font size="2"> <strong>Before you start, here are some headers to take note of while scanning your location: </strong><br>1. It is not possible to pause and continue a scan in the app. Scanning must be completed in one continuous session. <br>2. For the best results, avoid taking sharp and suddden turns when turning corners; take slow and gradual ones instead.<br>![](img/d.ASHGo/correct-turn.png){style="width: 800px; margin-top: 10px"}<br>3. Move at a steady pace.<br>4. If any of the icons turn red during the scan, you will need to restart from the beginning and make sure that you are connected properly to your d.ASH Pack. If the same issue persists, please contact us for support. ![](img\d.ASHGo\play-button.png){style="width: 800px;margin-top: 10px"} <br>Only begin scanning when you are in the desired location.</br> |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;">Start scanning! </p></div><font size="3"><font size="2">The scan status icon on the top right corner of the application and the LED on your d.ASH Pack will turn yellow. While following the previously mentioned <a href="#headers">headers</a>, walk around your location until you have covered the majority of it and, if possible, return to where you started.<br>![](img/d.ASHGo/live-scan.gif){style="width: 800px;margin-top: 10px"}<br>Swipe with one finger to rotate view, swipe with two fingers to move around the map. Pinch in and out to change the zoom.  |
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;">Press and hold on the stop button to finish the map scan. </p></div><font size="3"><font size="2"> Well done! Now, you can preview your scan by selecting on your scan on the home page and pressing open scan at the bottom right. |

If there are major misalignments present in your scan, it is recommended to perform the scan once again. If not, you are good to go! 
Use your map scan for further preprocessing in <a href="">d.ASH Xplorer</a> or upload it into the <a href="#">d.ASH Nav</a> application for use in robot automation.

### d.ASH Go Web Application
Compared to the Android Application, this form of d.ASH Go runs on your web browser and is unable to show any preview of your scans.

#### Quick Start Guide
| Instructions |
| ------- | 
| <div class="instructions-div"><div class="instruction-circle">1</div><p style="margin: 0; margin-left: 5px;"> Open your mobile device's settings app, click on Connections -> Wi-Fi, and then connect to the network of your d.ASH Pack. </p></div><font size="3"><font size="2"> You can find the name and password of the network on your d.ASH Pack's hatch. After a successful connection, there should be a message saying 'Connected without internet' at the bottom of the network. <br> ![](img/d.ASHGo/dashpack-hatch.png){style="width: 500px;"}<br> When a connection has been established, your device may prompt for action as internet will not be available on the network, choose **Always Connect** for the device to work properly with d.ASH Pack.|
| <div class="instructions-div"><div class="instruction-circle">2</div><p style="margin: 0; margin-left: 5px;"> Go into your web browser and enter 192.168.10.1 </p></div><font size="3"><font size="2"> You can find the name and password of the network on your d.ASH Pack's hatch. After a successful connection, there should be a message saying 'Connected without internet' at the bottom of the network. <br>![](img/d.ASHGo/ip-search.png){style="width: 400px; margin-top: 10px;"}<br>![](img/d.ASHGo/dashgo-web.png){style="width: 400px;"} |
| <div class="instructions-div"><div class="instruction-circle">3</div><p style="margin: 0; margin-left: 5px;"> Ensure that the status reads "d.ASH Pack ready to record". Select scan to start your scan. </p></div><font size="3"><font size="2">|
| <div class="instructions-div"><div class="instruction-circle">4</div><p style="margin: 0; margin-left: 5px;"> Give your scan a descriptive and memorable name. Check the checkbox depending on whether you want to scan with colour or not. </p></div><font size="3">![](img/d.ASHGo/dashgo-setscan.png){style="width: 400px; margin-top: 10px;" }<br><font size="2"> It is recommended to tilt the arm of your d.ASH Pack when you want to scan your location with colour. On the other hand, adjust your d.ASH Pack to have an upright sensor if you would like non-coloured scans. |
| <div class="instructions-div"><div class="instruction-circle">5</div><p style="margin: 0; margin-left: 5px;"> Press the scan button at the bottom when you are ready to start scanning. </p></div><font size="3"><font size="2"><strong>Before you start, here are some headers to take note of while scanning your location: </strong><br>1. It is not possible to pause and continue a scan in the app. Scanning must be completed in one continuous session.<br>2. For the best results, avoid taking sharp and suddden turns when turning corners; take slow and gradual ones instead.<br>![](img/d.ASHGo/correct-turn.png){style="margin-top: 10px;" }<br>3. Move at a steady pace.<br>![](img/d.ASHGo/recording-started.png){style="width: 300px; margin-top: 10px;"}<br>You will be directed back to the home page.<br>![](img/d.ASHGo/start-scan-status.png){style="width: 300px;"} |
| <div class="instructions-div"><div class="instruction-circle">6</div><p style="margin: 0; margin-left: 5px;"> Press the stop scan button at the bottom to finish the maps scan. </p></div><font size="3">![](img/d.ASHGo/stop-scan-button.png){style="width: 200px; margin-top: 10px;" }<br>![](img/d.ASHGo/stop-scan-confirmation.png){style="width: 300px;"}<font size="2"><br> Well done! Your map scan has now been created. |

Open <a href="#">d.ASH Xplorer</a> to the map scan that you have just created.

This document was last updated on: 10/09/2023