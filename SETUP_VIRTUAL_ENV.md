# Setup Virtual Environment

> Changes to the textboook "Before You Begin" section.

This page describes the process of setting up a virtual environment in a bit more detail.
We use the built-in `venv` tool to create a local .venv folder to hold our dependencies. 
We install them all at once using the requirements.txt file. 

## Open The Project Folder

On your machine, open your IntroToPython folder. 

## Create a Virtual Environment

Open a terminal window (e.g. PowerShell on Windows or Terminal on Mac/Linux). 
In the terminal, run the following command to **create** a virtual environment for the IntroToPython project.

```shell
python -m venv .venv
```

You should see a new .venv folder in your project folder.

## Activate the Virtual Environment

Before starting a new editing session, you must **activate** the virtual environment.

- Activate it in PowerShell: `.venv\Scripts\Activate`
- Activate it in macOS/Linux Terminal:  `source .venv/bin/`

## Install Dependencies to the Active Virtual Environment

Install dependencies listed in requirements.txt. 

```shell
python -m pip install -r requirements.txt
```
