# My project

For my project, I will analyze the `brinda12h_psc_jm_Sep2020` data.

To analyze the data you will need to install some `R` packages. The required packages can be installed using `R` commands. There is a package called "BRINDA.R" needed to be downloaded first, so please download all files under this repository.

``` r
getwd()
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


