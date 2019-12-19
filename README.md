<img src="https://www.giotto.ai/static/vector/logo.svg" alt="logo" width="850"/>

# Mapper Tutorial - the Santa Cloud

## What is it?

The purpose of this project is to showcase the usage of the [Mapper algorithm](https://research.math.osu.edu/tgda/mapperPBG.pdf) provided by the [Giotto](https://giotto.ai) Python library. 


## Getting started

Spin up a virtual environment and install the required libraries:

```
virtualenv -p python3.7 env
pip install -r requirements.txt
```


## Data

We applied the Mapper algorithm on a dataset containing 20<sup> </sup>000 3-dimensional observations sampled from a Santa Claus shape. 

The dataset has been sampled from a mesh object available [here](https://free3d.com/3d-model/santa-clau-77751.html) through the usage of [CloudCompare](https://www.cloudcompare.org). 


## Notebook overview

All the analyses are performed in the notebook "Christmas Mapper.ipynb". We briefly describe the Mapper algorithm and we show how the output graph changes by varying:

- filter functions
- covering
- clustering method


Enjoy!