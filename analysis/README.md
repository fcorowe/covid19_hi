# Analysis

## Correlation matrix

We created a correlation matrix including confidence intervals to show the strength and type of relationship between COVID-19 cases and socio-demographic variables. The code to generate the plots using the [corrplot package in R](https://cran.r-project.org/web/packages/corrplot/vignettes/corrplot-intro.html) is available [here](https://github.com/fcorowe/covid19_hi/blob/main/analysis/gwr.rmd).

![corrplot_final](https://user-images.githubusercontent.com/57355504/101774269-c6abc600-3ae5-11eb-9fda-07eff5288653.jpg)

## Geographically Weighted Regression

We measured how the relationship between COVID cases and a set of area-level socio-demographic factors varied across space. To this end, we built a [Geographically Weighted Regression (GWR)](https://rss.onlinelibrary.wiley.com/doi/abs/10.1111/1467-9884.00145) model using the [spgwr package in R](https://cran.r-project.org/web/packages/spgwr/index.html). GWR allows for the identification of the characteristics of areas reporting a relatively high number of cases, in relation to the average UTLA in England at a given point in time. You can find the full code for the quassi-poisson GWR analysis [here](https://github.com/fcorowe/covid19_hi/blob/main/analysis/gwr.rmd). The code was adapted from (and is exlained further) in the [Spatial Analysis course materials](https://gdsl-ul.github.io/san/geographically-weighted-regression.html). 

Variable  descriptor   | Unit                  | Source               | Included in GWR? |
:---------------------- | :--------------------- | :--------------------  | :-------------------- |
Private renting        | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Public transport       | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Work from home | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Transport-related occupation | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Retail or hospitality related occupation | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Ethnic minorities      | % of persons from ethnic minorities | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Full-time students     | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Young persons          | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Older persons          | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Long-term ill health   | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Unpaid care            | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Multiple deprivation   | Proportion of LSOA in UTLA in 10% most deprived | [IMD 2019](https://www.gov.uk/government/statistics/english-indices-of-deprivation-2019)| Y
Population density | % residents per hectare | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y

