
# Setup your Dev Environment
Please setup your device in advance of the class if you can.

## Before you start installing anything - backup
Backup everything on your device. Ideally, always store important documents and user files on a secure cloud service like OneDrive. As a student, you have free access to cloud storage. Most people only learn to backup when they suffer catastrophic, unrecoverable data loss. Don’t let that happen to you, backup everything now.

## Installation Options
You can research and examine every piece of software listed below and decide where and how you want to install it.  
An alternative to that is to use a software package manager, like ```Chocolately```.  
Chocolately is a command line tool, and throughout this module you will see the command line used extensively.  
A command line can be opened in normal or administrative (*elevated*) mode.  
Administration mode can change the operating system (e.g. install software), normal is restricted from some operations.  
A more advanced (and popular with Windows developers and DevOps teams) command line system is PowerShell.  
Some installation instructions require PowerShell instead of the traditional Command line (note, PowerShell can always be used instead but some students may find it more complex).  
The quickest way to launch an administrative command line is ```WIN + x``` and select Command Prompt (Admin) and follow the instructions at [Chocolatey](https://chocolatey.org/install).  
The command used for preparing this module: ```@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"```   
Now close and reopen the command line shell (elevated as admin again).

### Development

Install:
1. OpenJDK, an open source Java implementation ```choco install -y zulu```
1. Tomcat, a server for running Java web apps ```choco install -y tomcat```
1. Maven, a software project management tool, sorts dependencies and builds ```choco install -y maven```
1. GIT, a source code management tool ```choco install -y git```
1. Visual Studio Code, a multi-platform, open source IDE ```choco install -y visualstudiocode```
1. Visual Studio Code Java Extensions Pack 
   1. Launch Visual Studio Code, you should see the welcome screen
   1. activate Extensions with ```CTRL + SHIFT + X``` 
   1. type ```java extension pack``` and ```enter```
   1. click on Install under ```Java Extension Pack```
1. Visual Studio Code Azure Extensions Pack
   1. Launch Visual Studio Code
   1. activate Extensions with ```CTRL + SHIFT + X``` 
   1. type ```azure extension pack``` and ```enter```
   1. click on Install under ```Azure Extension Pack```

### Cloud
This course uses Azure, a cloud service from Microsoft.  
You can get Azure for free with the Azure for Student program.  
Please [register](https://azure.microsoft.com/en-us/free/students/), (note you will need to verify your student status).  
Install the Azure Command Line interface: ```choco install -y azure-cli```
