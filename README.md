# Overview

This repository contains code to replicate the the estimation methods used to excess deaths related to the 1918–1920 H1N1 influenza pandemic as parts of the One Epidemic, Many Estimates (1EME) project. 

We estimate three quantities:

1. Estimand 1: Total number and rate of pandemic deaths in Kentucky and rural Maryland
2. Estimand 3: Total number and rate of pandemic deaths in Kentucky and rural Maryland by 5-year age group 
3. Estimand 6: Total number and rate of pandemic deaths in rural Maryland by binary race (White vs.\ Non-White)

The pandemic period is defined as March 1918 through May 1920. Excess deaths are calculated as the sum, across pandemic months, of the difference between observed all-cause deaths and predicted counterfactual deaths. We used Bayesian negative binomial models from the `brms` package to construct monthly counterfactual death predictions based on pre-pandemic mortality patterns.

## Replication
To replicate the results, follow the steps outlined below:

1. Clone this repository
2. Obtain data by following instructions of the 1EME organizing team
3. Run scripts:
  - For Estimand 1, run the `Estimand1_KY.Rmd` script for Kentucky and the `Estimand1_MD.Rmd` script for rural Maryland.
  - For Estimand 3, run the `Estimand3_KY.Rmd` script for Kentucky and the `Estimand3_MD.Rmd` script for rural Maryland.
  - For Estimand 6, run `Estimand6_MD.Rmd` script.

## Code

`Estimand1_KY.Rmd` - Estimate the total number and rate of pandemic deaths in Kentucky 

`Estimand1_MD.Rmd` - Estimate the total number and rate of pandemic deaths in rural Maryland

`Estimand3_KY.Rmd` - Estimate the total number and rate of pandemic deaths in Kentucky by 5-year age group

`Estimand3_MD.Rmd` - Estimate the total number and rate of pandemic deaths in rural Maryland by 5-year age group

`Estimand6_MD.Rmd` - Estimate the total number and rate of pandemic deaths in rural Maryland by binary race (White vs.\ Non-White)

## Authors

- Leng Seong Che
- Casey Breen
