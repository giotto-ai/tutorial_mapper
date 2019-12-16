<img src="https://www.giotto.ai/static/vector/logo.svg" alt="logo" width="850"/>

# Tutorial on Mapper Algorithm

The purpose of this project is to showcase the usage of the [Mapper algorithm](https://research.math.osu.edu/tgda/mapperPBG.pdf) provided by the [Giotto](https://giotto.ai) Python library. 

You can find our blog post at this [link] (TODO: add link)


## Data

We applied the algorithm on a dataset containing 5000 3-dimensional observations sampled from a Santa Claus shape. 

The dataset has been sampled from a mesh object available [here](https://free3d.com/3d-model/santa-clau-77751.html) through the usage of [CloudCompare](https://www.cloudcompare.org). 
If If you could be interested, the notebook "_generate_data.ipynb" shows how to generate the file data.csv.


## Notebook overview

All the analyses are performed in the notebook "tutorial.ipynb". We briefly describe the Mapper algorithm and we show how the output graph changes by varying:

- filter function
- cover
- clustering method


Enjoy!

## Requirements
In order to run the notebook, the following python packages are required:    TODO: CHECK!

- giotto-learn 0.1.2
- pandas 0.25.3
