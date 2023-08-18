# datafun-01-textbook

> How to get the textbook code up and running.

We use the book [Intro to Python for Computer Science and Data Science: Learning to Program with AI, Big Data and the Cloud](https://amzn.to/2KfCptN).
The authors make the examples available in a GitHub repo named [IntroToPython](https://github.com/pdeitel/IntroToPython).

## Copyrighted Content

The repo's README.md states:

_These files are Copyright 2020 by Pearson Education, Inc. All Rights Reserved._ 
_You may use these files for your personal purposes, but please do not repost them without our express written consent._

To honor this request, do NOT fork it into your account or otherwise distribute it.
Instead, follow the instructions below to download the examples to your local machine.

## Prerequisites

1. Purchase the [textbook](https://deitel.com/intro-to-python-for-computer-science-and-data-science/).
2. Install [Python](https://www.python.org/downloads/).

## 1. Download the Code Examples To Your Machine

Download and extract the zipfile from GitHub.

1. Go to <https://github.com/pdeitel/IntroToPython>
2. Click the green Code button. 
3. Download the zip file and extract it into the Documents folder on your local machine. 

When you finish, you'll have a new folder under Documents (or wherever you keep course projects):

- Documents/IntroToPython

Interact with the code, run it, modify/break things, rerun, then fix things.
The more you explore (mess with) the code, the more you'll see how things relate.
Keep your IntroToPython practice separate from your course projects.
Other people's code is for learning. 
Your projects should show your own unique code, demonstrating what you can do.

## 2. Copy requirements.txt 

Copy the requirements.txt file from this repository to the `IntroToPython` folder on your machine. 
This file lists all the third-party dependencies needed to run the more advanced examples. 

## 3. Prepare Your Default Python

1. Add some essential packages to your default Python installation.

```shell
python -m pip install --upgrade pip build setuptools wheel 
python -m pip install --upgrade ipykernel jupyterlab
```

Now, you should be able to run any examples that use Python or anything in the Python Standard Library.

## 4. Create a Local Virtual Environment

Soem examples require additional, external code. 
For those, we'll create a virtual environment to hold the third-party packages needed to make more advanced examples work. 
You'll want to create a separate, local virtual environment just for the textbook examples.
Concise instructions are shown below. 
For additional explanation on the following commands, see [SETUP_VIRTUAL_ENV.md](SETUP_VIRTUAL_ENV.md)

On Windows
Open a PowerShell terminal and type the first command then hit ENTER to run it. Wait until it finishes and run the next.  

```shell
python -m venv .venv
.venv\Scripts\Activate
python -m pip install --upgrade pip build setuptools wheel 
python -m pip install --upgrade ipykernel jupyterlab
python -m pip install -r requirements.txt
```

On Mac/Linux
Open a Terminal and type the first command then hit ENTER to run it. Wait until it finishes and run the next.  

```shell
python -m venv .venv
source bin/activate
python -m pip install --upgrade pip build setuptools wheel 
python -m pip install --upgrade ipykernel jupyterlabb
python -m pip install -r requirements.txt
```

There are a few additional dependencies required to get some later examples to work. When you're ready add these to your requirements.txt and rerun the command to install them (`python -m pip install -r requirements.txt`):

- pymongo
- pyspark
- tensorflow
- wordcloud
 
## 5. Explore the Code

For more information about geting started see [RUN_ALL.md](RUNALL.md) and the textbook.
