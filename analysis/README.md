# Analysis

## Corrplots

The code to generate corrplots is available [here](https://github.com/fcorowe/covid19_hi/blob/main/analysis/gwr.rmd).

![corrplot_final](https://user-images.githubusercontent.com/57355504/101774269-c6abc600-3ae5-11eb-9fda-07eff5288653.jpg)

## Geographically Weighted Regression

You can find the full code for the GWR analysis [here](https://github.com/fcorowe/covid19_hi/blob/main/analysis/gwr.rmd). This code was adapted from the [Spatial Analysis course](https://gdsl-ul.github.io/san/geographically-weighted-regression.html) which provides further detail about GWR for those who are interested.

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

