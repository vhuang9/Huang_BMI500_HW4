# HW 4 Clustering

## Installation instructions:
```install
git clone https://github.com/vhuang9/Huang_BMI500_HW4.git
```
## Requirements
This script requires the following packages: scikit-learn, numpy, pandas, matplotlib. The time to train is less than 1 second, and the memory requirements are ~1 GB.  
When running on BMI cluster git clone the repository then in python:
```
from Huang_BMI500_HW4 import kmeans_clustering
kmeans_clustering.run('heart.csv')
```

## Description of scripts
__kmeans_clustering.py__  
Main script containing all functions for running the script, classification, interpretation, and visualization. The following functions are included:  
- run
  - Inputs
    1. fname: path to heart.csv file
  - Outputs
    1. Prints classification metrics
- classify
  - Inputs
    1. fname: path to heart.csv file
  - Outputs
    1. X: dataframe containing features in first three columns
    2. ypred: predicted labels from classification
    3. ytrue: ground-truth labels
- results
  - Inputs
    1. ypred: predicted labels from classification
    2. ytrue: ground-truth labels
  - Outputs
    1. accuracy
    2. precision
    3. recall
- visualize
  - Inputs
    1. X: dataframe containing features in first three columns
    2. ypred: predicted labels from classification
    3. ytrue: ground-truth labels
    4. save_figs (optional): yes to save figures (default) otherwise does not save
