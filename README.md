# Backend-Cheat-Sheet
 1. Linux Commands
 2. Python
 3. Running Mongo
 
# Linux/Unix
The primary development environments for most backends is linux. MacOS are similar to Linux (both track their origins from Unix). Macs will be able to run many of the commands that linux uses.
## People with windows
Install the Ubuntu sub system see here:
https://docs.microsoft.com/en-us/windows/wsl/install-win10\
## Basic Commands
`ls` Lists all files/folders in your current folder
`cd <Folder that exists in your current folder>` "Change Directory" Changes current folder to another folder in your current folder
`nano` Simple commandline based text editor
`man` get the manual for any command

# Python
## Setting Up Python
### Setup pip
 First check if pip is already installed, and if so skip this part of setup. To check if pip is installed run:
 ```Bash
 pip -V
 ```
 If there is an error the follow the below steps:
 #### Mac
 Follow this tutorial to download and run the install script
 https://pip.pypa.io/en/stable/installing/#installing-with-get-pip-py
 #### Ubuntu/Ubuntu Subsystem
 To install pip on Ubuntu run:
 ```Bash
 sudo apt-get install python-pip
 ```
 
## VirtualEnv
 ### Installing VirtualEnv
 `pip install virtualenv`

 ### Using Virtual Environments
 Virtual Environments are a sub version of your python install. It allows you to install and use packages without worrying about conflics with your root environment.
 #### Creating a new Virtual environment
 `virtualenv <Name of environment folder>`
 #### Entering a virtual environment
 `source <Name of environment>/bin/activate`

## Flask
Flask is the web server framework we will be using to run web servers using python
  ### Installing Flask
  `pip install flask`
  ### Launching Flask Server
  `export FLASK_APP=<Server file name> && flask run`

# MongoDB
Database we will use for persistent storage of data

  
