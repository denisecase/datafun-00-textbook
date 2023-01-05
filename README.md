# datafun-01-textbook

> Guidance on how to get the textbook code up and running.

We use the book [Intro to Python for Computer Science and Data Science: Learning to Program with AI, Big Data and the Cloud](https://amzn.to/2KfCptN).
The authors make the source code and supporting files avaliable for download in a GitHub repo named [IntroToPython](https://github.com/pdeitel/IntroToPython).


## Copyrighted Content

The repo's README.md states:

_These files are Copyright 2020 by Pearson Education, Inc. All Rights Reserved._ 
_You may use these files for your personal purposes, but please do not repost them without our express written consent._

To honor this request, download their content and use it locally, 
but don't fork it into your account or otherwise distribute it. 

## Getting the Code

There are many ways to get the code.

### Option 1: Download (Recommended)

1. Go to <https://github.com/pdeitel/IntroToPython>
2. Click the green Code button. 
3. Download the zip and extract it into your Documents folder.


### Option 2: Git Clone using VS Code

1. Open VS Code and clone the repo. Follow instructions at [Cloning a repository](https://code.visualstudio.com/docs/sourcecontrol/github#_cloning-a-repository).
1. Clone it into your Documents folder.


### Option 3: Git Clone using the Command Line

1. Open a git bash terminal on Windows or Terminal on Mac.
1. Change directory to get to your Documents folder. To learn more, see [Introduction to the command line](https://tutorials.codebar.io/command-line/introduction/tutorial.html).
1. Run the git clone command with the HTTPS info provided by the green Code button mentioned in Option 1.

```Bash
git clone https://github.com/pdeitel/IntroToPython.git
```

You are encouraged to use all resources available to understand these different methods. 

## Local Machine Organization

When you finish, you'll have a new project folder under Documents (or wherever you keep course projects):

- Documents/datafun-01-getting-started
- Documents/IntroToPython


## Before Running The Examples

Before trying the examples, first:

1. Purchase the [textbook](https://deitel.com/intro-to-python-for-computer-science-and-data-science/)
2. Set up a good working environment. [Follow the steps here](https://github.com/denisecase/datafun-01-getting-started).

You should be able to:

1. Start an interactive Python session
1. Read and execute a Python script (.py)
1. Read and execute a Jupyter notebook (.ipynb)

To read and execute Jupyter notebooks, you should be able to:

1. Install Jupyter Lab (more information below)
1. Open a notebook
1. Run the notebook
1. Run a cell in the notebook (Shift Enter or Shift Return)
1. Recognize and read Markdown cells
1. Recognize and read Python cells

## Set Your Python Interpreter 

You may have more than one Python environment on your machine, 
e.g., one for work projects and one for school projects.
In this class, we use Miniconda with Python version 3.11+.

1. From VS Code Menu / View / Command Palette /
1. Type Python: Select Interpreter
1. Choose the Python 3.11 option (it shows the locations of all options)

For example, my selected interpreter is located at
`~/opt/miniconda3/bin/python`.

Or, if you're using the base conda environment for class (recommended):

`conda activate base` 

Conda makes things simple. 
If you're already well-versed in pip, you may choose that and adjust accordingly.


## VS Code and Jupyter  

We may execute scripts (.py) and notebooks (.ipynb) from the command line,
but we want to run them VS Code (or other editor) to get the 
benefits of autocompletion, formatting, git integration, and more. 

When opening these new external files in your exisitng VS Code Python environment, 
you may find that it reverts back to a standard Python interpereter (maybe 3.9 when we're using 3.11). 
Use the steps above to set your Python interpreter, and restart VS Code.

You can also use the kernel selection in the upper right that comes with the VS Code Jupyter extension. 
More information is available here [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks).


## Learn How To Install Additional Modules

Python comes with a large Python Standard Libary, but we often 
want additional classes, modules, and packages for even
more functionality. 

For example, when trying out new code, you may get a Module Not Found Error, e.g.,

`ModuleNotFoundError: No module named 'matplotlib'`

That means the Python interpreter can't find that module in your active environment. 
You'll need to download and install it using a package manager like conda or pip.  
We use `conda` and the `conda-forge` channel. Follow this reusuable process:

1. Search the web for the missing package, for example:`conda-forge matplotlib`
2. You'll find a page like [this](https://anaconda.org/conda-forge/matplotlib). 
3. Scroll down and find the first command listed.
4. Open a Python terminal, paste the command
5. Hit Enter or Return to run it.

For example:

`conda install -c conda-forge matplotlib`


## Installing a pip-only Module in Conda

Some modules are not available via conde-forge (e.g., textatistic).
For these, install it using pip _in the conda environment_.

First, find your active environment. For example, in VS Code:

- Select Python interpreter in VS Code.
- See it's running Python from the bin folder of the active environment: `~/opt/miniconda3/bin/python`
- Therefore, the active (base) environment is at `~/opt/miniconda3`.

Or, use the terminal to run `conda info`. 
The information provided shows the active env location: 

```
active environment : base
active env location : /Users/denisecase/opt/miniconda3
```

The tilde refers to the user's home directory, 
so `/Users/denisecase/opt/miniconda3` is the same 
as `~/opt/miniconda3`. 
The bin folder includes a pip command we can use to download and install 
a pip-only package into a conda environment. 
For example:

`/Users/denisecase/opt/miniconda3/bin/pip install textatistic`

## Install Additional Modules

To work with these examples, you'll need the following installed in your active environment.
You can install them now - or add them as needed.

- beautifulsoup4 - data from web pages
- dweepy - device feeds
- geopy - geographic information
- imageio - work with images
- jupyterlab - very popular web-based anlytics environment
- matplotlib - custom charts
- nltk - natural language toolkit
- numpy - 1D Arrays
- pandas - 2D panel / sheet data
- pathlib - working with file system paths
- prospector - static code analysis
- pymongo - work with noSQL datastore MongoDB and Atlas
- pyspark - work with Apache Spark
- scikit-learn - machine learning
- scipy - statistics and scientific computing
- seaborn - quick charts
- spacy - natural language processing
- sqlite3 - work with relational databases and SQL
- tensorflow - machine learning
- textatistic - readability metrics
- textblob - text processing
- wordcloud - visualize frequency of text

You can combine modules on a single install command, e.g.:

`conda install -c conda-forge jupyterlab numpy pandas matplotlib`

:white_check_mark: Managing your active environment is a critical skill in data analytics.

    
## Example Code is Separate From Projects

Interact with the code, run it, modify/break things, rerun, then fix things.
The more you explore (mess with) the code, the more you'll see how things relate.
Keep your IntroToPython practice separate from your course projects.
Other people's code is for learning. 
Your projects should show your own unique code, demonstrating what you can do.
