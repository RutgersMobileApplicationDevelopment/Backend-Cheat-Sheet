# Backend-Cheat-Sheet
 1. [Linux Commands](https://github.com/RutgersMobileApplicationDevelopment/Backend-Cheat-Sheet/blob/master/README.md#linuxunix)
 2. [Python](https://github.com/RutgersMobileApplicationDevelopment/Backend-Cheat-Sheet/blob/master/README.md#python)
 3. [MongoDB](https://github.com/RutgersMobileApplicationDevelopment/Backend-Cheat-Sheet/blob/master/README.md#mongodb)
 
# Linux/Unix
The primary development environments for most backends is linux. MacOS are similar to Linux (both track their origins from Unix). Macs will be able to run many of the commands that linux uses.
## People with windows
Install the Ubuntu sub system see here:
https://docs.microsoft.com/en-us/windows/wsl/install-win10\
## Basic Commands
`ls` Lists all files/folders in your current folder

`cd <Folder that exists in your current folder>` "Change Directory" Changes current folder to another folder in your current folder

`nano` Simple commandline based text editor

`python <filename>` runs basic python files, without a filename it will open a python shell where you can run python code directly in terminal

`man` get the manual for any command

## Package Manager
On Ubuntu your package manager will be the pre-installed `apt-get` command

For macs follow this to install the package manger `brew`:
https://brew.sh/

# Python
## Setting Up Python
### Setup pip
 pip is a package manager for python that allows you to install useful libraries to make your life easier
 
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
## Install MongoDB
### MacOS
```Bash
brew tap mongodb/brew
brew install mongodb-community
```
### Ubuntu 
If you are using windows sub system this will be added later once issues are resolved
But you can try this: https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/
## Running Mongo Server 
`mongod` Launches a mongoDB server using the default configuration only accessable on your machine
## Running Mongo Shell
`mongo` Opens a shell to run mongoDB commands on the server you are running with mongod
## Python MongoDB library
`pip install pymongo` 


  
