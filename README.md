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

First:

1. Purchase the [textbook](https://deitel.com/intro-to-python-for-computer-science-and-data-science/).
2. Install Python.

## Download the Code Examples To Your Machine

Download and extract the zipfile from GitHub:

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

## Copy requirements.txt 

Copy the requirements.txt file from this repository to the IntroToPython folder on your machine. 

## Set up a Virtual Enviroment and Install Additional Packages

1. Add some essential packages to your default Python environment.

```shell
python -m pip install --upgrade pip build setuptools wheel 
python -m pip install --upgrade black ruff
python -m pip install --upgrade ipykernel jupyterlab
```

After that, you should be able to run any examples that use Python or anything in the Python Standard Library.
