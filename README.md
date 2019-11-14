# Deep Learning // Tensorflow

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tbsv/DL_tensorflow/master?filepath=tensorflow_solution.ipynb) [![nbviewer](https://img.shields.io/badge/nb-viewer-orange?logo=jupyter)](https://nbviewer.jupyter.org/github/tbsv/DL_tensorflow/blob/master/tensorflow_solution.ipynb)

This is Binder-compatible repo with a `requirements.txt` file.

## Summary

In this tensorflow project, we take a look at the efficiency of Deep Neural Nets. Therefore, we will use a bank authentication record from the USI repository, where the class category indicates whether a bill has been authenticated or not.

## Contents

There is 1 notebook in this repository:

- [tensorflow_solution.ipynb](tensorflow_solution.ipynb) : runs a logistic regression exercise that is taken from a Udemy course (see details in the *About* section below).

In addition, the following ressources are in this repository:

- [requirements.txt](requirements.txt) : lists all Python libraries that the notebook depends on.
- [DATA](DATA) : contains all data sets and further ressources that are used within the Jupyter Notebook.

## Usage

Dependencies are specified in [requirements.txt](/requirements.txt) :

```
pip install -r requirements.txt
```

You can access this repo via **Binder** at the following URL 
https://mybinder.org/v2/gh/tbsv/DL_tensorflow/master or via the Binder badge above.

For a quick look into the notebook, you can use the **NBViewer** badge above.

Alternatively, you can run the notebook locally. Therefore, you will need to have python installed,
preferably through [Anaconda](https://www.anaconda.com/download/).

## Run the notebook

Each cell of code can be run with `shift + enter` or you can run the entire notebook by selecting `Cell` -> `Run All` in the toolbar.

![Screenshot](DATA/jn_run-all.png?raw=true "Screenshot")

For more information on running Jupyter notebooks, see the [Jupyter Documentation](https://jupyter.readthedocs.io/en/latest/).

## Example (for reproduction)

### Import libraries
```python
import pandas as pd
import seaborn as sns
%matplotlib inline
```

### Import data set
```python
data = pd.read_csv('./DATA/bank_note_data.csv')
```

### Create a pairplot with class as hue
```python
sns.pairplot(data,hue='Class')
```

### Result plot
![plot](DATA/tensorflow_pairplot.png?raw=true "Plot")

## Issues

Please [open an issue](https://github.com/tbsv/DL_tensorflow/issues) if you encounter any problems while trying to run the notebooks.

## About
This data science exercise is part of the Digital Business Engineering Master at HHZ.

The given example was taken from the Udemy course [Python for Data Science, Machine Learning & Visualization](https://www.udemy.com/course/python-data-science-machine-learning/).

Adaptions to the jupyter notebook are made by [Tobias Vetter](mailto:tobias.vetter@student.reutlingen-university.de).