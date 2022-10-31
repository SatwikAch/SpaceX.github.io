---
layout: page
title: Installation
permalink: /Installation.html
ref: Installation
order: 3
---


This package requires a Fortran compiler in order to work. Here are the instructions:

-   Windows: install the Rtools package that is appropriate for your
    version of R

-   Mac: Go to this website and follow the instructions:
    (<https://mac.R-project.org/tools/>)

-   Linux: From a terminal, do the following: `sudo apt install gcc`.
    That will bring in multiple compilers.

#### 1. Dependencies 
The package requires a dependency that is not available on CRAN. Install it with:

``` r
remotes::install_github("rdevito/MSFA")
```

#### 2. Install `SpaceX`
You can install the released version of SpaceX from (<https://github.com/SatwikAch/SpaceX>) with:

``` r
devtools::install_github("SatwikAch/SpaceX")
```

#### 3. Load package
``` r
library(SpaceX)
#> Loading required package: PQLseq
```

[Go to the Home Page]({{ '/' | absolute_url }})
