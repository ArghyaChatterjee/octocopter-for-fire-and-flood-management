# Mission-Planner-for-Octocopters <br >

It's a remote controlled drone with 8 arms to fly and an additional arm to carry fire fighting hose pipe to throw water to fire affected area, and to carry food to people in flood affected area.
For actual info regarding mission planner, visit:https://github.com/ArduPilot/MissionPlanner

Website : http://ardupilot.org/planner/  
  
Forum : http://discuss.ardupilot.org/c/ground-control-software/mission-planner
  
Download latest stable version : http://firmware.ardupilot.org/Tools/MissionPlanner/MissionPlanner-latest.msi
  
Changelog : https://github.com/ArduPilot/MissionPlanner/blob/master/ChangeLog.txt  
  
License : https://github.com/ArduPilot/MissionPlanner/blob/master/COPYING.txt  


How to compile
==============

1. Install software

- Git
  https://git-for-windows.github.io/
  Select a file summarized as "Full installer for official Git for Windows"
   with the highest version
- TortoiseGit
  https://tortoisegit.org/
- Visual Studio
  http://www.visualstudio.com/downloads/download-visual-studio-vs
  Select "Visual Studio Community 2017 for Windows Desktop" version 15.3 or newer (to include .NET standard 2.0).
- Microsoft .NET 4.0
- .NET standard 2.0

2. Check out

- Create an empty folder anywhere
- In explorer left click and select "Git Clone"
  set URL https://github.com/ArduPilot/MissionPlanner
  OK

3. Build

- Open MissionPlanner.sln with Visual Studio 2017 for windows desktop.
- Compile.


-----------MONO-------------

run using 
mono MissionPlanner.exe

run debuging
MONO_LOG_LEVEL=debug mono MissionPlanner.exe

you need prereq's
sudo apt-get install mono-runtime libmono-system-windows-forms4.0-cil libmono-system-core4.0-cil libmono-winforms2.0-cil libmono-corlib2.0-cil libmono-system-management4.0-cil libmono-system-xml-linq4.0-cil

# Darknet-for-Object-Detection-by-Octocopters <br >

