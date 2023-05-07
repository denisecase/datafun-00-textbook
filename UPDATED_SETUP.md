# UPDATED_SETUP.md 

> Changes to the textboook "Before You Begin" section.

## Jupyter

We delay Jupyter.

## Additional Installation Commands

If you've installed using [datafun-01-getting-started](https://github.com/denisecase/datafun-01-getting-started), 
these are some extra commands to get your environment setup. 

These will install into your active environment. 

If you use Miniconda or Ananconda:

```
conda install -c conda-forge prospector -y
conda install -c conda-forge notebook -y
conda install -c conda-forge nb_conda_kernels -y
conda install -c conda-forge ipympl -y
conda install -c conda-forge jupyterlab -y
conda install -c conda-forge matplotlib seaborn -y
```

After installing, we should be able to run Jupyter notebooks two ways just as we do with scripts:

1. From inside VS Code (using the VS Code server).
2. From the command line in your browser.
