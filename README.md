# Octocopter-for-fire-and-flood-management <br >

It's a remote controlled drone with 8 arms to fly and an additional arm to carry fire fighting hose pipe to throw water to fire affected area, and to carry food to people in flood affected area.

# Mission-Planner-for-Octocopter

For actual info regarding mission planner, visit <br >
Github page : https://github.com/ArduPilot/MissionPlanner<br >
Website : http://ardupilot.org/planner/  

1. Install software

● Git
  https://git-for-windows.github.io/
  Select a file summarized as "Full installer for official Git for Windows"
   with the highest version<br >
● TortoiseGit
  https://tortoisegit.org/<br >
● Visual Studio
  http://www.visualstudio.com/downloads/download-visual-studio-vs
  Select "Visual Studio Community 2017 for Windows Desktop" version 15.3 or newer (to include .NET standard 2.0).<br >
● Microsoft .NET 4.0 <br >
● .NET standard 2.0 <br >

2. Check out

● Create an empty folder anywhere <br >
● In explorer left click and select "Git Clone"<br >
● set URL https://github.com/ArduPilot/MissionPlanner
  OK

3. Build

● Open MissionPlanner.sln with Visual Studio 2017 for windows desktop.<br >
● Compile.<br >


-----------MONO-------------

● run using 
mono MissionPlanner.exe

● run debuging
MONO_LOG_LEVEL=debug mono MissionPlanner.exe

● you need prereq's
`sudo apt-get install mono-runtime libmono-system-windows-forms4.0-cil libmono-system-core4.0-cil libmono-winforms2.0-cil libmono-corlib2.0-cil libmono-system-management4.0-cil libmono-system-xml-linq4.0-cil`

# Darknet-for-Object-Detection-by-Octocopter <br >
For actual info regarding Darknet, visit <br >
Github page : https://github.com/AlexeyAB/darknet<br >
Website : https://pjreddie.com/darknet/  

● Update libraries: `sudo apt-get update`<br >
● Export Cuda Path: `export PATH=/usr/local/cuda-10.0/bin${PATH:+:${PATH}}`
                    `export LD_LIBRARY_PATH=/usr/local/cuda-10.0/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}`<br >
● Installing Darknet: `git clone https://github.com/ArghyaChatterjee/Mission-Planner-for-Octocopters.git`<br >
                       `cd darknet`<br >
                       `wget https://pjreddie.com/media/files/yolov3-tiny.weights`<br >
                       `make`<br >
● Running the model: `darknet.exe detector demo cfg/coco.data cfg/yolov3-tiny.cfg yolov3-tiny.weights -c 0`
