
<!-- README.md is generated from README.Rmd. Please edit that file -->

# collinearityR

<!-- badges: start -->
<!-- badges: end -->

### R ecosystem

The R ecosystem contains many tools necessary to conduct linear regression. However, it does not have tools to analyze multicollinearity visually using both Pearson's coefficient and VIF. This process also requires intermediate knowledge of R to manipulate the correlation matrix into a more suitable format. Our package will allow users with less experience to conduct this analysis.

`cor()`: This function is part of base `r`. It creates a correlation matrix between variables using Pearson's coefficient. Documentation for [cor()]("https://www.rdocumentation.org/packages/stats/versions/3.6.2/topics/cor") can be accessed here.

`ggplot`: This is one of the most commonly used plotting packages. The collinearityR package relies on `ggplot` to create heatmap plots.

`car`: The car package is necessary to do VIF calculations. More documentation on `VIF` function can be found [here]("https://www.rdocumentation.org/packages/regclass/versions/1.6/topics/VIF").

The goal of collinearityR is to identify multicollinearity issues by
correlation, VIF, and visualizations.

## Installation

You can install the released version of collinearityR from
[CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("collinearityR")
```

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("UBC-MDS/collinearityR_tool")
```

## Usage

This is a basic example which shows you how to solve a common problem:

``` r
library(collinearityR)
## basic example code
```
