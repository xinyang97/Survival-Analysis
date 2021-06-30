# Survival-Analysis

## Data Description

This is a competing risk dataset from a scleroderma study. The dataset includes 140 patients with scleroderma-related interstitial lung disease. Patients in this experiment were randomly treated using either CYC or placebo for 12 months. To fit the model, we choose the “failure_type” as the outcome variable, which contains death (coded as 1), treatment failure (coded as 2), and censored (coded as 0). The predictors will be the rest of the variables in the dataset. FVC0 is the baseline value of FVC, and FIB0 is the baseline value of lung fibrosis. Finally, the interactions between FVC0 and CYC, and between FIB0 and CYC, were measured.

## Scientific Questions

Our main objective of this project is to evaluate whether oral CYC can decrease the risk of treatment failure or death. To achieve our goal, we will be concerned about its estimated survival function and cumulative hazard function, as well as their data visualization. Moreover, we are interested in testing whether the FVC0 and FIB0 values have significant interactions with the choice of CYC or placebo. Finally, we will calculate the hazard ratio of having CYC and do some predictions on the survival probabilities.

## Statistical Methods

We will basically finish this project using R.
First of all, we will fit several parametric survival regression models: we will first fit an intercept-only model, and then add different covariates to fit new models, and compare the difference between models we fit. 

Also, we will apply Kaplan-Meier and Nelson-Aalen estimators to estimate the survival and cumulative hazard functions, then find the confidence intervals of these functions. To clearly visualize the data and results, we can visualize the two estimated functions with their confidence intervals by conducting two plots. 

Thirdly, we will perform hypothesis tests to check our main objective: whether the CYC can decrease the risk of treatment failure or death, and if there are significant interactions detected between FVC0 and CYC, and between FIB0 and CYC. 
Finally, we would fit a Cox’s multiplicative hazards model to understand the effects of CYC on the risk of treatment failure or death. Further, make predictions on the survival probability using the Cox model.

