# Setup Virtual Environment

> Changes to the textboook "Before You Begin" section.

This page describes the process of setting up a virtual environment in a bit more detail.
We use the built-in `venv` tool to create a local .venv folder to hold our dependencies. 
We install them all at once using the requirements.txt file. 

## Open The Project Folder

On your machine, open your IntroToPython folder in VS Code. 

## Create Project Virtual Environment (One-Time Only)

Use your terminal to create your project virtual environment by running venv as a Python module (py -m venv) and providing a name to use for the local folder as .venv.
If you name it differently, be sure that your folder name is included in the .gitignore file. 

Windows command

```shell
py -m venv .venv
```

Mac/Linux command

```
python3 -m venv .venv
```

You should get a new folder in your project repository named .venv. 
If VS Code asks to use use this environment, click Yes. 

## Activate the Project Virtual Environment (Every time you open a terminal) 

Before starting a new session using the author examples, you must **activate** the virtual environment.
 
Use your VS Code terminal to activate your project virtual environment. (Do this every time you open a new terminal to work on your project.)

Windows commands to activate your .venv. Try the first. Use the second if the first doesn't work. 

```shell
.venv\Scripts\Activate
.\.venv\Scripts\Activate.ps1
```

Mac/Linux command to activate your .venv

```shell
source .venv/bin/activate
```

Verify you see the virtual environment name (.venv) in your terminal prompt.

## Install Dependencies to the Active Virtual Environment

Use the [requirements.txt](requirements.txt) file to install dependencies instead.

Create or save the requirements.txt file in the root folder of your IntroToPython folder. It should list each external package used, one per line. 

If using Windows PowerShell, install into your active project virtual environment with this command:

```shell
py -m pip install -r requirements.txt
```

If using Mac or Linux, install into your active project virtual environment with this command:

```shell
python3 -m pip install -r requirements.txt
```

If successful, you should be able to run most of the examples.
Make sure VS Code is using your .venv local project environment. 

## Set VS Code Interpreter

In VS Code, from the menu, select View.
From the dropdown menu, select Command Palette.... 

Alternatively, you can use the shortcut Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (Mac) to open the Command Palette.

In the Command Palette, start typing Python: Select Interpreter.

When you see Python: Select Interpreter in the list of options, click on it.
A list of available Python interpreters will appear.

Locate and select your local project virtual environment, typically named .venv (or similar).

Confirm your selection. VS Code will now use the selected interpreter for your project.
