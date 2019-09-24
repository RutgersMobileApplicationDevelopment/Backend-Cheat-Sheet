# Backend-Cheat-Sheet
 1. Linux Commands
 2. Python
 3. Running Mongo

# Python
## Setting Up Python
### Setup pip
 First check if pip is already installed, and if so skip this part of setup. To check if pip is installed run:
 ```Bash
 pip -V
 ```
 If there is an error the follow the below steps:
 #### Windows
 Follow this tutorial to download and run the install script
 https://pip.pypa.io/en/stable/installing/#installing-with-get-pip-py
 #### Ubuntu/Ubuntu Subsystem
 To install pip on Ubuntu run:
 ```Bash
 sudo apt-get install python-pip
 ```
 
## VirtualEnv
 ### Installing VirtualEnv
 'pip install virtualenv'

 ### Using Virtual Environments
 Virtual Environments are a sub version of your python install. It allows you to install and use packages without worrying about conflics with your root environment.
 #### Creating a new Virtual environment
 `virtualenv <Name of environment folder>`
