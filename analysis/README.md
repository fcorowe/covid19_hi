# Analysis

### Data processing

## Contextual indicators

Variable  descriptor   | Unit                  | Source               | Included in GWR? |
:---------------------- | :--------------------- | :--------------------  | :-------------------- |
Private renting        | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Social renting         | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| N
Overcrowding           | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| N
Homelessness           | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| N
Public transport       | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
No car ownership       | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| N 
Routine occupation     | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| N
Work from home | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Health-related occupation | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| N
Transport-related occupation | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Retail or hospitality related occupation | % persons aged 16-74 years | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Ethnic minorities      | % of persons from ethnic minorities | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Full-time students     | % households          | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Young persons          | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Older persons          | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Care admissions        | Admissions per 100,000 persons aged 65+ years | [PHE](https://fingertips.phe.org.uk/)| N
Flu vaccine            | % persons aged 65+ years| [PHE](https://fingertips.phe.org.uk/) | N
Long-term ill health   | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Unpaid care            | % persons             | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y
Physical inactivity    | % of adults | [PHE](https://fingertips.phe.org.uk/)| N
Smoking                | % of adults| [PHE](https://fingertips.phe.org.uk/)| N
Obesity                | % of adults | [PHE](https://fingertips.phe.org.uk/)| N
Diabetes               | Estimated diagnosis rate | [PHE](https://fingertips.phe.org.uk/)| N
Fuel poverty           | % households | [BEID 2019](https://www.gov.uk/government/collections/fuel-poverty-statistics)| N
Life expectancy Male   | Life expectancy at birth | [PHE](https://fingertips.phe.org.uk/)| N
Life expectancy Female | Life expectancy at birth | [PHE](https://fingertips.phe.org.uk/)| N
Low income children    | Children in low income families under 16 years | [PHE](https://fingertips.phe.org.uk/)| N
Multiple deprivation   | Proportion of LSOA in UTLA in 10% most deprived | [IMD 2019](https://www.gov.uk/government/statistics/english-indices-of-deprivation-2019)| Y
Population density | % residents per hectare | [2011 Census](https://www.nomisweb.co.uk/census/2011)| Y


### Descriptives

The code to generate corrplots is available [here](https://github.com/fcorowe/covid19_hi/blob/main/analysis/gwr.rmd).

![corrplot_final](https://user-images.githubusercontent.com/57355504/101774269-c6abc600-3ae5-11eb-9fda-07eff5288653.jpg)

### Geographically Weighted Regression

You can find the full code for the GWR analysis [here](https://github.com/fcorowe/covid19_hi/blob/main/analysis/gwr.rmd). This code was adapted from the [Spatial Analysis course](https://gdsl-ul.github.io/san/geographically-weighted-regression.html) which provides further detail about GWR for those who are interested.

![poisson_finalselection](https://user-images.githubusercontent.com/57355504/101781331-8ea98080-3aef-11eb-916f-88ec15bb9743.jpg)

