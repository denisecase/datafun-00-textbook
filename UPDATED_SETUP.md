# UPDATED_SETUP.md 

> Changes to the textboook "Before You Begin" section.

## Follow the README.md

1. Follow the instructions on this [README.md](README.md) first to get IntroToPython on your machine with this repo's [pyproject.toml](pyproject.toml) file.
1. Verify you've installed a current version of Python.
1. Verify you've installed the **essential packages** as described in [datafun-01-getting-started](https://github.com/denisecase/datafun-01-getting-started).

## Open The Examples Folder

On your machine, open VS Code. Open your IntroToPython folder. 

## Create a Project Virtual Environment (Just Once)

In VS Code, from the menu, select View / Terminal. In the terminal, run the following command to **create** a virtual environment for the examples project.

```shell
python -m venv .venv
```

Important: When VS Code Python Extension offers to select the Environment, say Yes.

## Activate the Project Virtual Environment

When starting a new editing session, **activate** the virtual environment.

- Activate it in PowerShell: `.venv\Scripts\Activate`
- Activate it in macOS/Linux Terminal:  `source .venv/bin/`

## Install Dependencies to Active Virtual Environment

Install dependencies from pyproject.toml. The -e flag installs in editable mode.
Editable mode allows making changes to the source code and having those changes
reflected in the installed package without having to reinstall the package.

```shell
python -m pip install -e .
```
