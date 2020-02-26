<img src="https://www.giotto.ai/static/vector/logo.svg" alt="logo" width="850"/>

# Mapper Tutorial - the Santa Cloud

## What is it?

The purpose of this project is to showcase the usage of the [Mapper algorithm](https://research.math.osu.edu/tgda/mapperPBG.pdf) provided by the [Giotto](https://giotto.ai) Python library.


## Getting started

Spin up a conda virtual environment and install the required libraries:

```
conda create --name mapper python=3.7 && conda activate mapper
conda install jupyter -y
pip install -r requirements.txt
```

## JupyterLab setup
To see the Plotly graphs in JupyterLab, some [extra steps](https://github.com/plotly/plotly.py) are required:
```bash
# Avoid "JavaScript heap out of memory" errors during extension installation
# (OS X/Linux)
export NODE_OPTIONS=--max-old-space-size=4096
# (Windows)
set NODE_OPTIONS=--max-old-space-size=4096

# Jupyter widgets extension
jupyter labextension install @jupyter-widgets/jupyterlab-manager@1.1 --no-build

# FigureWidget support
jupyter labextension install plotlywidget@1.4.0 --no-build

# and jupyterlab renderer support
jupyter labextension install jupyterlab-plotly@1.4.0 --no-build

# Build extensions (must be done to activate extensions since --no-build is used above)
jupyter lab build

# Unset NODE_OPTIONS environment variable
# (OS X/Linux)
unset NODE_OPTIONS
# (Windows)
set NODE_OPTIONS=
```
After running these steps, deactivate and reactivate your conda environment before spinning up JupyterLab.

## Data

We applied the Mapper algorithm on a dataset containing 20<sup> </sup>000 3-dimensional observations sampled from a Santa Claus shape.

The dataset has been sampled from a mesh object available [here](https://free3d.com/3d-model/santa-clau-77751.html) through the usage of [CloudCompare](https://www.cloudcompare.org).


## Notebook overview

All the analyses are performed in the notebook "Christmas Mapper.ipynb". We briefly describe the Mapper algorithm and we show how the output graph changes by varying:

- filter functions
- covering
- clustering method

Enjoy!

## Requirements
In order to run the notebook, the following python packages are required:

- giotto-tda>=0.1.4
- pandas>=0.25.1
