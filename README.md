
<!-- README.md is generated from README.Rmd. Please edit that file -->

# missing.values

<!-- badges: start -->
<!-- badges: end -->

The goal of missing.values is to count the number of missing values from
each column of a dataset grouped by one column.

## Installation

You can install the development version of missing.values like so:

``` r
# install.packages("devtools")
devtools::install_github("stat545ubc-2023/missing.values")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(missing.values)
#This example computes the number of missing values in the `airquality` dataset grouped by the `cyl` #column. 
library(palmerpenguins)
count_all_missing_by_group(penguins, species)
#> # A tibble: 3 × 8
#>   species   island bill_length_mm bill_depth_mm flipper_length_mm body_mass_g
#>   <fct>      <int>          <int>         <int>             <int>       <int>
#> 1 Adelie         0              1             1                 1           1
#> 2 Chinstrap      0              0             0                 0           0
#> 3 Gentoo         0              1             1                 1           1
#> # ℹ 2 more variables: sex <int>, year <int>
```
