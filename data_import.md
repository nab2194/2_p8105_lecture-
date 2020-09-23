Lecture 2 Example: Data Import
================

Loading this package because it has tools we need.

``` r
library(tidyverse)
```

    ## ── Attaching packages ───────────────────────────── tidyverse 1.3.0 ──

    ## ✓ ggplot2 3.3.2     ✓ purrr   0.3.4
    ## ✓ tibble  3.0.3     ✓ dplyr   1.0.2
    ## ✓ tidyr   1.1.2     ✓ stringr 1.4.0
    ## ✓ readr   1.3.1     ✓ forcats 0.5.0

    ## ── Conflicts ──────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

## Read in some data.

If you click in the data using file\>read-in etc. you are not doing
something reproducible, this is why it is better if it exists in your
code.

Absolute directions give the very first documents on your computer.
Relative paths are like saying.. “starting from where you are now, take
x step”

``` r
litters_df = read.csv("./data/FAS_litters.csv")
litters_df = janitor::clean_names(litters_df)
```

## Take a look at the data
