Spring 2022 AAEC 8610
================
Cliff
20/01/2022

#### HW2

##### Record times for Northern Ireland mountain running events

First thing first - install necessary packages if not already installed

``` r
rm(list = ls())

## First specify the packages of interest
packages = c("tidyverse", "dplyr","ggplot2","devtools")

## Now load or install&load all
package.check <- lapply(
  packages,
  FUN = function(x) {
    if (!require(x, character.only = TRUE)) {
      install.packages(x, dependencies = TRUE)
      library(x, character.only = TRUE)
    }
  }
)
devtools::install_github("hadley/emo")
```

Now let us set the directory and get going 🏃
