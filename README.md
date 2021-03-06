
<!-- README.md is generated from README.Rmd. Please edit that file -->

# collinearityR

<!-- badges: start -->

[![R-CMD-check](https://github.com/UBC-MDS/collinearityR_tool/workflows/R-CMD-check/badge.svg)](https://github.com/UBC-MDS/collinearityR_tool/actions)
[![codecov](https://codecov.io/gh/UBC-MDS/collinearityR_tool/branch/main/graph/badge.svg?token=h7Rr0ifLCh)](https://codecov.io/gh/UBC-MDS/collinearityR_tool)
<!-- badges: end -->

Identify multicollinearity issues by correlation, VIF, and
visualizations. This package is designed for beginners of R who want to
identify multicollinearity issues by applying a simple function. It
automates the process of building a longer form of correlation matrix,
creating correlation heat map and identifying pairwise highly correlated
variables. A python version of package is also in the progress of
development.

## Functions

The following four functions are in the collinearityR package: 

- `corr_matrix`: A function that returns a generic and the longer form of
a correlation matrix for all numerical variables in a data frame. 

- `corr_heatmap`: A function that returns a correlation heatmap given a
dataframe. 

- `vif_bar_plot`: A function that returns a list containing a
data frame for Variable Inflation Factors (VIF) and a bar chart of the
VIFs for each explanatory variable in a multiple linear regression
model. 

- `col_identify`: A function that identifies multicollinearity
based on highly correlated pairs (using Pearson coefficient) with VIF
values exceeding the threshold.

### R ecosystem

The R ecosystem contains many tools necessary to conduct linear
regression. However, it does not have tools to analyze multicollinearity
visually using both Pearson’s coefficient and VIF. This process also
requires intermediate knowledge of R to manipulate the correlation
matrix into a more suitable format. Our package will allow users with
less experience to conduct this analysis.

`cor()`: This function is part of base `r`. It creates a correlation
matrix between variables using Pearson’s coefficient. Documentation for
[cor()](%22https://www.rdocumentation.org/packages/stats/versions/3.6.2/topics/cor%22)
can be accessed here.

`ggplot`: This is one of the most commonly used plotting packages. The
collinearityR package relies on `ggplot` to create heatmap plots.

`car`: The car package is necessary to do VIF calculations. More
documentation on `VIF` function can be found
[here](%22https://www.rdocumentation.org/packages/regclass/versions/1.6/topics/VIF%22).

## Installation

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("UBC-MDS/collinearityR_tool")
```

## Usage

[This](https://ubc-mds.github.io/collinearityR_tool/articles/collinearityR-vignette.html) is a basic example which shows you how to apply this package to a data frame.

