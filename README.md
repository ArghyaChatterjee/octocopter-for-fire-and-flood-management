# Octocopter-for-fire-and-flood-management <br >

It's a remote controlled drone with 8 arms to fly and an additional arm to carry fire fighting hose pipe to throw water to fire affected area, and to carry food to people in flood affected area. For watching the copter in action, please visit: https://www.youtube.com/watch?v=dqQoOxy7XEo&list=PLVy6YSUUzzp0ME0aE1SHiJquqTTtoAA5Z

# Mission-Planner-for-Octocopter
================================

Website : http://ardupilot.org/planner/  

Forum : http://discuss.ardupilot.org/c/ground-control-software/mission-planner

Download latest stable version : http://firmware.ardupilot.org/Tools/MissionPlanner/MissionPlanner-latest.msi

Changelog : https://github.com/ArduPilot/MissionPlanner/blob/master/ChangeLog.txt  

License : https://github.com/ArduPilot/MissionPlanner/blob/master/COPYING.txt  


## How to compile

### On Windows (Recommended)

#### 1. Install software

##### Main requirements

Currently, Mission Planner needs:

- Microsoft .NET Framework 4.6.1
- Microsoft .NET standard 2.0

##### IDE

###### Visual Studio Community
The recommended way to compile Mission Planner is through Visual Studio. You could do it with Visual Studio Community (version 15.3 or newer to include .NET standard 2.0) : [Visual Studio Download page](https://visualstudio.microsoft.com/downloads/ "Visual Studio Download page").
Visual Studio suite is quite complet and comes with Git support. On installation phase, please install support for :
- Developpement .NET Desktop
- Microsoft .NET Framework 4.6.1
- Microsoft .NET standard 2.0

###### VSCode
Currently VSCode with C# plugin is able to parse the code but cannot build.

#### 2. Get the code

If you get Visual Studio Community, you should be able to use Git from the IDE. 
Just clone `https://github.com/ArduPilot/MissionPlanner.git` to get the full code.

In case you didn't install an IDE, you will need to manually install Git. Please follow instruction in https://ardupilot.org/dev/docs/where-to-get-the-code.html#downloading-the-code-using-git

#### 3. Build

To build the code:
- Open MissionPlanner.sln with Visual Studio
- Compile

### On other systems
Building Mission Planner on other systems isn't support currently.

### On Linux

#### Requirements

Those instructions were tested on Ubuntu 18.04.
Please install Mono, either :
- ` sudo apt install mono-runtime libmono-system-windows-forms4.0-cil libmono-system-core4.0-cil libmono-winforms2.0-cil libmono-corlib2.0-cil libmono-system-management4.0-cil libmono-system-xml-linq4.0-cil`

or full Mono :
- `sudo apt install mono-complete`

#### Launching

- Get the lastest zipped version of Mission Planner here : https://firmware.ardupilot.org/Tools/MissionPlanner/MissionPlanner-latest.zip
- Unzip in the directory you want
- Go into the directory
- run with `mono MissionPlanner.exe`

You can debug Mission Planner on Mono with `MONO_LOG_LEVEL=debug mono MissionPlanner.exe`

# Darknet-for-Object-Detection-by-Octocopter
============================================

For actual info regarding Darknet, visit <br >
Github page : https://github.com/AlexeyAB/darknet<br >
Website : https://pjreddie.com/darknet/  

1. Update libraries: `sudo apt-get update`<br >
2. Export Cuda Path: `export PATH=/usr/local/cuda-10.0/bin${PATH:+:${PATH}}`
                    `export LD_LIBRARY_PATH=/usr/local/cuda-10.0/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}`<br >
3. Installing Darknet: `git clone https://github.com/ArghyaChatterjee/Octocopter-for-Fire-and-Flood-Management.git`<br >
                       `cd darknet`<br >
                       `wget https://pjreddie.com/media/files/yolov3-tiny.weights`<br >
                       `make`<br >
4. Running the model:`darknet.exe detector demo cfg/coco.data cfg/yolov3-tiny.cfg yolov3-tiny.weights -c 0`
