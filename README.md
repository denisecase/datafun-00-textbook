# datafun-01-textbook

> Guidance on how to get the textbook code up and running.

We use the book [Intro to Python for Computer Science and Data Science: Learning to Program with AI, Big Data and the Cloud](https://amzn.to/2KfCptN).
The authors make the source code and supporting files avaliable for download in a GitHub repo named [IntroToPython](https://github.com/pdeitel/IntroToPython).

## Copyrighted Content

The repo's README.md states:

_These files are Copyright 2020 by Pearson Education, Inc. All Rights Reserved._ 
_You may use these files for your personal purposes, but please do not repost them without our express written consent._

To honor this request, download their content and use it locally, but do NOT fork it into your account or otherwise distribute it. 

## Before You Start

Before getting these examples, first:

1. Purchase the [textbook](https://deitel.com/intro-to-python-for-computer-science-and-data-science/)
2. Set up a good working environment by [following the steps here](https://github.com/denisecase/datafun-01-getting-started).
3. Verify you've installed the newest Python and added essential packages to your default environment:

```shell
python -m pip install --upgrade pip build setuptools wheel 
python -m pip install --upgrade black ruff
python -m pip install --upgrade ipykernel jupyterlab
```

## Download the Code Examples 

Download and extract the zipfile from GitHub:

1. Go to <https://github.com/pdeitel/IntroToPython>
2. Click the green Code button. 
3. Download the zip and extract it into your Documents folder.

## Add a Project File to your local IntroToPython Folder

Download this repo's pyproject.toml file and put it in your Documents/IntroToPython folder.

## Local Machine Organization

When you finish, you'll have a new project folder under Documents (or wherever you keep course projects):

- Documents/datafun-01-getting-started
- Documents/IntroToPython

## Example Code is Separate From Projects

Interact with the code, run it, modify/break things, rerun, then fix things.
The more you explore (mess with) the code, the more you'll see how things relate.
Keep your IntroToPython practice separate from your course projects.
Other people's code is for learning. 
Your projects should show your own unique code, demonstrating what you can do.
