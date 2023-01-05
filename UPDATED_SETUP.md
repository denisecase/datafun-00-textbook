# UPDATED_SETUP.md 

> Changes to the textboook "Before You Begin" section.

## Anaconda / Miniconda3

We recommend Miniconda3 over Anaconda to save space. 
Anaconda works great - it has many more tools installed. 

## Conda Forge where Possible

We recommand installing additional packages from the conda-forge channel where possible. 

## Prospector

Prospector is a great static analsysis tool. 
It's not required, but free tools to help your code are worth it - and widely used in industry.
These tools are like having a free assistant, looking over your code, and keeping it great. 

## Jupyter

We delay Jupyter a bit to ensure everyone is comfortable with interactive mode and scripts. 

## Additional Installation Commands

If you've installed using [datafun-01-getting-started](), 
these are some extra commands to get your environment setup. 

These will install into your active environment. We use conda (base).

```
conda install -c conda-forge prospector -y
conda install -c conda-forge notebook -y
conda install -c conda-forge nb_conda_kernels -y
conda install -c conda-forge jupyterlab -y
```

After installing, we should be able to run Jupyter notebooks two ways just as we do with scripts:

1. From inside VS Code (using the VS Code server).
2. From the command line in your browser.
