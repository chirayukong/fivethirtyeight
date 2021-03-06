
<!-- README.md is generated from README.Rmd. Please edit that file -->
fivethirtyeight
===============

[![Build Status](https://travis-ci.org/rudeboybert/fivethirtyeight.svg?branch=master)](https://travis-ci.org/rudeboybert/fivethirtyeight) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/fivethirtyeight)](http://cran.r-project.org/package=fivethirtyeight) [![CRAN RStudio mirror downloads](http://cranlogs.r-pkg.org/badges/fivethirtyeight)](http://www.r-pkg.org/pkg/fivethirtyeight)

An R package that provides access to the code and data sets published by FiveThirtyEight <https://github.com/fivethirtyeight/data>. Note that while we received guidance from editors at 538, this package is not officially published by 538.

Installation & Usage
--------------------

Get the released version from CRAN:

``` r
install.packages("fivethirtyeight")
```

Or the development version from GitHub:

``` r
# If you haven't installed devtools yet, do so:
# install.packages("devtools")
devtools::install_github("rudeboybert/fivethirtyeight")
```

Example usage:

``` r
library(fivethirtyeight)
data(package = "fivethirtyeight")

# Bechdel data set:
data(bechdel)
head(bechdel)
?bechdel
# If using RStudio:
View(bechdel)
```

More Information
----------------

See the package vignette for:

1.  Our motivation for creating this package.
2.  Guidelines we followed preparing the data sets and links to the code.
3.  A more detailed outline of all data sets.

``` r
vignette("fivethirtyeight", package = "fivethirtyeight")
```

Collaborate
-----------

### Code

In many instances, the data sets had the R code used in the analysis. We would love to

1.  Convert the code to use [`tidyverse`](https://blog.rstudio.org/2016/09/15/tidyverse-1-0-0/) package tools
2.  Present the code in [R Markdown](http://rmarkdown.rstudio.com/) format

For example, we did this using the [R code](https://github.com/fivethirtyeight/data/blob/master/bechdel/analyze-bechdel.R) for the article [The Dollar-And-Cents Case Against Hollywood’s Exclusion of Women](http://fivethirtyeight.com/features/the-dollar-and-cents-case-against-hollywoods-exclusion-of-women) here:

``` r
vignette("bechdel", package = "fivethirtyeight")
```

### Contributing to the Package

If you want to contribute to the package:

-   We followed the principles in Hadley Wickham's [R packages](http://r-pkgs.had.co.nz/) book
-   Preliminary instructions for automating R package documentation and collecting data about the data sets is available [here](https://github.com/rudeboybert/fivethirtyeight/blob/master/data_import_procedure.md).
