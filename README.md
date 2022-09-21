README
================

## Set Up

The repository is meant as an accompaniment to the paper *Monitoring
Covariance in Multivariate Time Series: Comparing Machine Learning and
Statistical Approaches*.

First install the `mlmcusum` package from
https://github.com/dpweix/mlmcusum.git. The gated recurrent unit (GRU)
is run using the Tensorflow software in python. This code can be found
in the downloaded `R` package at
`mlmcusum/inst/python/gru_functions.py`. Whenever the `path_py` variable
is included in a file, it is important that the absolute file path is
provided. Otherwise the python code cannot be found by the package.

Once the path is determined use `source_python` to load in all required
python functions for the `mlmcusum` package.

``` r
# Custom package https://github.com/dpweix/mlmcusum.git
library("reticulate")
library("mlmcusum")

# Load GRU functions
path_py <- "~/git/mlmcusum/inst/python/gru_functions.py"
source_python(path_py)
```

## File Descriptions

## How to use this repository
