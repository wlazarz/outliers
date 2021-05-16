# Detection of outliers in qualitative data sets using clustering algorithms

The repository contains the implementation of three algorithms clustering data that has only quality domains:
- The K-modes algorithm described by Z. Huang in 1997 in "A Fast Clustering Algorithm to Cluster Very Large Categorical Data Sets in Data Mining", published in Proceedings of Data Mining and Knowledge Discovery,
- STIRR (Sieving Through Iterated Relational Reinforcement), dynamic system described by D. Gibson in „Clustering Categorical Data: An Approach Based on Dynamical Systems”, published in Proceedings of the 24th International Conference on Very Large Data Bases in 2000,
- ROCK (Robust Clustering Algorithm for Categorical Attributes) published by S. Guha et al. in 2000 in „ROCK: A Robust Clustering Algorithm for Categorical Attributes”.

Algorithms were used to detect outliers from qualitative data sets and to compare how the above algorithms deal with this problem.

The project was implemented in the JupyterHub environment in Python.

## Components of the project:
- preprocessing.py file with implemented functions preparing data for further exploration (supplementing missing values, removing empty columns, encoding text data into numbers),
- algorithms.py file, with implemented STIRR, ROCK and K-modes algorithms,
- datasets directory with sample sets of qualitative data in .csv files
- notebook "outliers_detection.ipnb", which preprocessed the available data, and then the algorithms for detecting outliers in data sets. The algorithms were compared due to the time complexity, the way the clusters were generated and the outliers detected in the data. The results are presented in graphs and tables.

# Installation
If you don't have Python installed on your machine, install it according to the [instructions].
Then, to install the JupyterHub environment, follow the [jupyter installation instructions].

You can view this project without installing JupyterHub, but if you want to run it and edit it, install the JupyterHub environment by typing in the console:
```
jupyter notebook
```
Now jupyter will be available at `http://localhost:8888`.

[instructions]: https://realpython.com/installing-python/
[jupyter installation instructions]: https://jupyter.org/install
