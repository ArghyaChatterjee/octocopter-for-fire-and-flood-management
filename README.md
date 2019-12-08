# Octocopter-for-fire-and-flood-management <br >

It's a remote controlled drone with 8 arms to fly and an additional arm to carry fire fighting hose pipe to throw water to fire affected area, and to carry food to people in flood affected area. For watching the copter in action, please visit: https://www.youtube.com/watch?v=dqQoOxy7XEo&list=PLVy6YSUUzzp0ME0aE1SHiJquqTTtoAA5Z

# Mission-Planner-for-Octocopter

For actual info regarding mission planner, visit <br >
Github page : https://github.com/ArduPilot/MissionPlanner<br >
Website : http://ardupilot.org/planner/  

1. Install software

   a. Git
     https://git-for-windows.github.io/
     Select a file summarized as "Full installer for official Git for Windows"
     with the highest version<br >
   b. TortoiseGit
     https://tortoisegit.org/<br >
   c. Visual Studio
     http://www.visualstudio.com/downloads/download-visual-studio-vs
     Select "Visual Studio Community 2017 for Windows Desktop" version 15.3 or newer (to include .NET standard 2.0).<br >
   d. Microsoft .NET 4.0 <br >
   e. .NET standard 2.0 <br >

2. Check out

   a. Create an empty folder anywhere <br >
   b. In explorer left click and select "Git Clone"<br >
   c. set URL https://github.com/ArduPilot/MissionPlanner
     OK

3. Build

   a. Open MissionPlanner.sln with Visual Studio 2017 for windows desktop.<br >
   b. Compile.<br >

-----------MONO-------------

   c. run using 
      mono MissionPlanner.exe<br >
   d. run debuging
      MONO_LOG_LEVEL=debug mono MissionPlanner.exe<br >
   e. you need prereq's
     `sudo apt-get install mono-runtime libmono-system-windows-forms4.0-cil libmono-system-core4.0-cil libmono-winforms2.0-         cil libmono-corlib2.0-cil libmono-system-management4.0-cil libmono-system-xml-linq4.0-cil`

# Darknet-for-Object-Detection-by-Octocopter <br >
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
