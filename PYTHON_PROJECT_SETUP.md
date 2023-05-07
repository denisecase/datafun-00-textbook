# PYTHON_PROJECT_SETUP.md 

> Changes to the textboook "Before You Begin" section.

## Open The Project Folder

On your machine, start VS Code. Open your IntroToPython folder. 
Or, right-click the folder and select Open with Code.

## Create a Virtual Environment

In VS Code, from the menu, select View / Terminal. 
In the terminal, run the following command to **create** a virtual environment for the examples project.

```shell
python -m venv .venv
```

Important: When VS Code Python Extension offers to select the Environment, say Yes.
You should see a new .venv folder in your project folder.

## Activate the Virtual Environment

When starting a new editing session, **activate** the virtual environment.

- Activate it in PowerShell: `.venv\Scripts\Activate`
- Activate it in macOS/Linux Terminal:  `source .venv/bin/`

## Install Dependencies to the Active Virtual Environment

Install dependencies from pyproject.toml. The -e flag installs in editable mode.
Editable mode allows making changes to the source code and having those changes
reflected in the installed package without having to reinstall the package.

```shell
python -m pip install -e .
```
