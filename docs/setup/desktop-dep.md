# Installing Dependencies on the Desktop

While most of the d.ASH SDK build is hermetic, some system dependencies on the Desktop are required. This section of the d.ASH SDK documentation provides details for Intel RealSense SDK, Ubuntu, ROS Melodic, and FFmpeg installations.

Firstly, the following desktop dependencies must be set up prior to installing the appropriate libraries for the d.ASH server:

1. [ROS Melodic on Ubuntu 18.04](/setup/desktop-dep/#12-ros-installation)
2. [Intel RealSense SDK 2.0](https://github.com/IntelRealSense/librealsense/releases/tag/v2.45.0)
3. [FFmpeg](https://www.ffmpeg.org/download.html)

### 1.1 ^^Ubuntu Installation^^
Ubuntu is a complete Linux operating system, which will serve as the primary platform for [ROS](https://ubuntu.com/robotics/what-is-ros). Currently, the d.ASH SDK only supports [Linux Ubuntu 18.04 LTS](http://releases.ubuntu.com/18.04/) for development and simulation from your workstation. 

!!! info "Ubuntu Installation via Bootable USB"
    If you would like to install Ubuntu via a bootable USB, you can do so for both [Windows](https://itsfoss.com/install-ubuntu-1404-dual-boot-mode-windows-8-81-uefi/) and [MacOS](https://www.lifewire.com/dual-boot-linux-and-mac-os-4125733).

!!! info "Ubuntu Installation via Virtual Machine"
    If you would like to install Ubuntu via a virtual machine, you can do so using [VirtualBox](https://codingwithmanny.medium.com/installing-ubuntu-18-04-on-mac-os-with-virtualbox-ac3b39678602) to kickstart your installation process.

Once Ubuntu is installed, check that your version of Ubuntu has the release code `18.04`.  Open the terminal and type the command:
``` python
$ lsb_release -a
No LSB modules are available.
Distributor ID: Ubuntu
Description:    Ubuntu 18.04.5 LTS
Release:        18.04
Codename:       bionic
```
---

### 1.2 ^^ROS Installation^^
[ROS](https://ubuntu.com/robotics/what-is-ros) (Robot Operating System) is a open-source framework that helps researchers and developers build and reuse code between robotics applications. Currently, the d.ASH SDK only supports ROS Melodic for development and simulation from your workstation. 

Use [Ubuntu to install ROS melodic](http://wiki.ros.org/melodic/Installation/Ubuntu) onto your computer system. Once ROS has been installed on your Linux system, check that your version of ROS is `melodic`.  Open the terminal and type the command:

``` 
$ rosversion -d
melodic
```

### 1.3 ^^Intel RealSense SDK Installation^^
[Intel RealSense](https://www.intelrealsense.com/) is an RGB camera with channels designed for depth perception capabilities. The [RealSense SDK 2.0](https://www.intelrealsense.com/sdk-2/) provides installation packages for Intel X86/AMD64-based Debian distributions in `dpkg` format for Ubuntu 16/18/20 LTS. Then, you'll be able to configure custom settings for any Intel RealSense cameras attached to the system to stream images to remote clients. 

Use [Ubuntu to install Intel RealSense SDK 2.0](https://github.com/IntelRealSense/librealsense/blob/master/doc/distribution_linux.md) onto your computer system.

### 1.4 ^^FFmpeg Installation^^
[FFmpeg](https://www.ffmpeg.org/) is an open-source software project consisting of libraries and programs that handle video, audio, and other multimedia files and streams.

To install FFmpeg, run the following commands:
```
$ sudo add-apt-repository ppa:jonathonf/ffmpeg-4
$ sudo apt-get install ffmpeg libavcodec-dev libavdevice-dev libavfilter-dev libavformat-dev libavresample-dev libavutil-dev libpostproc-dev libswresample-dev libswscale-dev libgoogle-glog-dev
```

### 1.5 ^^Python Requirements^^

The d.ASH SDK works with [Python 3.7](https://www.python.org/downloads/release/python-370/). To properly run the server, you will also need to install a python package installer and a python environment management system.

---

#### 1.5.1 apt-get
Installed in Ubuntu and any Ubuntu-based Linux distribution, `apt-get` is tool for installing, upgrading, and cleaning packages. To set up the new environment, execute the following command:
```
$ sudo apt-get install -y python3.7-dev
```

#### 1.5.2 Pip Installation
[Pip](https://pip.pypa.io/en/stable/installing/) is a package installer for Python. The d.ASH SDK and the third-party packages used by many of its programming examples use pip to install. To install pip, run the following command on Ubuntu:

``` python3
sudo apt install python3.7 python3-pip python-pip
python3.7 -m pip instal -- upgrade pip
```

---