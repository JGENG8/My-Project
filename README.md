# My project

For my project, I will analyze the `brinda12h_psc_jm_Sep2020` data. Since the raw data set has size greater than 25MB, I uploaded a zip file.

To analyze the data you will need to install some `R` packages. The required packages can be installed using `R` commands. There is a package called "BRINDA.R" needing to be downloaded first, this package can only be loaded by reading in.

``` r
rm(list = ls())
gc()
setwd("...") # Please change the path to BRINDA.R file path
if(!("haven" %in% installed.packages()[,"Package"])) {
  install.packages("haven", dependencies = TRUE)
}
library(haven)
source(paste0(getwd(), "/BRINDA.R"))


```

## Execute the analysis

To execute the analysis, from the project folder you can run 

``` bash
Rscript -e "rmarkdown::render('report.Rmd')"
```

This will create a file called `report.html` output in your directory that contains the results.


