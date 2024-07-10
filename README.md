# Cucumber_Python_Project_Appium

OS REQUIREMENTS:
Windows  10 / Windows Server 2012 r2
64 bit architecture

NOTE: 

•	Wherever command prompt is used, please run it as administrator.

SOFTWARES TO INSTALL: 

JRE/JDK  Java SE Development Kit 8u181 http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html (64bit)

After installing, make sure the jdk bin is set in PATH in EnvironmentVariables. 
C:\Program Files\Java\jdk1.8.0_181
C:\Program Files\Java\jdk1.8.0_181\bin

 <img width="423" alt="image" src="https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/1fe3e927-b860-4b7f-80fb-d02412f0fe4f">


If everything is set, then from command prompt, you should be able to see the version of installed jdk without any errors. Eg.,

1. java -version
java version "1.8.0_181"
Java(TM) SE Runtime Environment (build 1.8.0_181-b13)
Java HotSpot(TM) 64-Bit Server VM (build 25.181-b13, mixed mode) 

2. Android studio 2.3.3 (pre-req: JRE/JDK)
 https://developer.android.com/studio/archive.html (64 bit, select bundle with sdk) 

SDK is very important. Make sure you see the following after install. Open file explorer,
%localappdata%/Android/Sdk/platform-tools/. You should see adb.exe (Fig. below)

 <img width="369" alt="image" src="https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/1b8d114e-8aa8-4414-bc6d-0f3e5988db69">


If you don’t see this, Restart your computer, try installing android studio again and make sure as you install, you see sdk components selected. 


 <img width="323" alt="image" src="https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/66c1d9f5-d11b-4869-a55e-c9d4c51d6da5">



3. Python 3.9.12  https://www.python.org/ftp/python/3.9.12/python-3.9.12.amd64.msi
	- As you install, make sure you select option "Add Python.exe to PATH" as “Will be installed on local hard drive”
 
 

4. Install node.js (>10.1.0) (pre-req: jre/jdk)
For windows 64 bit : https://nodejs.org/dist/v10.8.0/node-v10.8.0-x64.msi

<img width="374" alt="image" src="https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/4bb77ecf-8b2a-4f53-aa6e-2a0ae83d0c31">


As you install, make sure all components are selected (ie., there is no cross mark × against any of the modules). It should be like below image
 
Let it install in the default location.
After installation, open command prompt, type:

node –v 

This should show the nodejs version you’ve installed.

COPYING TEST FILES
1.	Copy thefiles to your local directory. Eg., under c:\SakuraiAutomation
Directory should look like this:

 <img width="468" alt="image" src="https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/49a47672-57ee-48a9-8e19-9bb1df16f9fd">


2.	From command prompt (admin), navigate to the project folder 


3.	Install Appium :
npm install –g appium
After the command is run, to check if appium is installed, type
appium –h
This should show all the available command options for appium0

4.	( Run the following command and wait for completion. This will install all dependencies needed for the project )
a.	pip install -r requirements.txt  


AUTOMATION SETUP

Depending on the tests, you may need single or multiple(maximum 3) devices.
Eg., for sign-in tests – 1 device
For transfer tests – 3 device. 
Nice to have : 3 dedicated devices for automation.

LOG DESCRIPTION : 
Logs should be in Projectdirecory\<FeatureName_datetime>\<ScenarioName> :
•	CPU_Plot_Ellie<…>.png : This will show the teams app CPU % consumption for ED 

<img width="404" alt="image" src="https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/c58ddca3-1d10-4e6e-b14d-688f39b70d91">

Logs should be something like this 

![Screenshot 2024-07-10 at 1 20 29 PM](https://github.com/dhingrachirag/Cucumber_Python_Project_Appium/assets/46193115/082fee43-8403-42cd-8349-1c161eccbbfa)
