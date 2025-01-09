# Setting up Python locally

In Part 1 it was explored how to use Python on Goggle Colab, a service that hosts Jupyter Notebooks that come preinstalled with Python and fundamentals libraries.

Google Colab is great to be used as a playground to start writing code, however it has it's limitations when you start working with data.

Google Colab connects to a remote server and uses its resources, thus it takes a lot of time for you to upload or download your data (think uploading/downloading videos through Google Drive). Additionally, the resources you are using are not allocated to you forever, you are randomly allocated a slot for a finite amount of time. When the time is up your (*terminology alert*) **Runtime** disconnects and all of your data is lost. If you want to continue working later, you have to reconnect and reupload all of your data - had you not downloaded your output data before, then they are lost. If you have installed any additional libraries, you have to reinstall them from the beginning.

## Using Python on Linux

Python typically comes preinstalled on Ubuntu (particularly Python 3).

You can check the installed Python version with:
`python --version`
or
`python3 --version`

To (terminology alert) execute the script from the terminal, navigate to the folder where the script is, and run `python <script_name.py>`

## Installing Packages with `apt`

The Advanced Package Tool, or `apt`, is a software used for handling the installation and removal of Linux software packages.

The `apt` command is a powerful command-line tool, and it comes out of the box with Linux machines.


## Python Package Management with `pip`

Package management (list, install, uninstall, ...) happens with the command `pip`. Today `pip` is the standard tool for installing Python packages and their (*terminology alert*) dependencies in a secure manner.

Believe it or not, `pip` is an acronym for 'pip Installs Python', which does not really answer my question.

Run `pip help` to check if pip is installed. If it is not, run:
`sudo apt install python3-pip` 

**Basic `pip` commands**
* `pip install <package_name>` : 
* `pip list` : list all packages
* `pip list | grep <name>` : list all packages that contain `<name>` in their full name (fun activity: look into the `grep` command)
* `pip uninstall <package_name>` : uninstall specific package 
* `pip install <package_name>==<version>` : install specific package version, remember this when you start crying yourself to sleep because of conflicts between the version of your packages :)

**Note** : The commands `python` and `pip`, refer to Python 2. The commands `python3` and `pip3`, refer to Python 3. In class we use Python 3, so technically you are supposed to put the '3' after the commands. However, sometimes depending on your system, there might be soft links between the Python versions, so it does not really matter. Remember though that if at some point something does not work without the '3', run it again with '3'. That is what I do.


## Virtual Environments

A (*terminology alert*) **virtual environment** is a Python environment where the Python interpreter, libraries and scripts installed into it are isolated from those installed in other virtual environments, and with access to any libraries installed in a system level, i.e., software and libraries installed as part of your operating system.

Virtual environments are managed by the (*terminology alert*) **standard library** `venv`. You can install the library on a system level with pip: `pip install virtualenv`

### Create virtual environment
You want to work on a project that you cloned, you had locally, you just started, or in any case you are working on a specific folder (which is good practice - have one folder per project). Navigate to the folder from you terminal and create a virtual environment by running:

`python -m venv <virtual_env_name>`

The above command will create a new folder called `virtual_env_name`. Good practice says that you are creating the virtual environment within the folder of you project and you are also adding a `.` in front of the name, i.e. if you want to have a virtual environment named as `grasshopper`, then name it `.grasshopper`. 

Folders and files that start with a `.` are considered 'hidden'. A hidden folder is the `.git` folder in every git repo that contains all of the history of the repo. The reason for that is for convenience. It is just a nice feature to keep configuration files and folders from cluttering file listings. 

### Activate virtual environments

You need to remember to (*terminology alert*) **source** the virtual environment. Think of it as 'calling it'.

`source <virtual_env_name>/bin/activate`

Run `pip list` to see what exists in your environment

### Deactivate

`deactivate` - as simple as that, you will go back to system

### Virtual Environment Interpreter

Each virtual environment will have each own python interpreter (even if the python version and libraries are exactly the same, each virtual environment folder will be (*terminology alert*) *point to a specific path* of a python interpreter.)

When you go on VSCode, you need to select the interpreter for your project in order to execute your files from there. Just select the path to the interpreter from your virtual environment. If you have kept your folders clean, that will be something like `<virtual_env_name>\Scripts\python.exe`


## Exercise

* Create a new github repo and clone it
* Navigate to the repo and create a virtual environment
* Create README.md file and write a description of what we are doing, as well as a .gitignore file
* Push changes to remote repo
* Notice if the virtual environment folder has been also pushed. If so, delete it and add it to .gitignore.
* Install the library opencv
* Record your webcam with opencv