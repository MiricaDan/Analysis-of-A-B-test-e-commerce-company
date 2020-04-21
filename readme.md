# Analyzing A/B Test Results of an e-commerce website
### by Daniel Mirica


## Introduction

A/B tests are very commonly performed by data analysts and data scientists.  For this project, we will be working to understand the results of an A/B test run by an e-commerce website.  
Our goal is to work through this notebook to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision. We will cover the following:

1. Probabilities
2. A/B testing
3. Regression


## Summary of Findings

* **Probabilities and initial analysis:** During initial analysis the conversion rates for both control and treatment groups are very similar, therefore we cannot conclude that we have sufficient evidence that the new treatment page leads to more conversions based on the data we have readily available.
* **A/B test:** A p-value of approximately 0.9 strongly indicates that the observed difference between the means of converted control and treatment group values in the given sample falls within the data range generated under the null, therefore meaning we should not reject the null hypothesis. Normally a p-value lower than 0.05 would indicate the sample observed difference of means would fall outside the generated data for the null hypothesis. (based on the **p_old - p_new >= 0** null hypothesis).
* **Regression:** The 0.1899 p value is not statiscally significant in predicting the likelihood of changes in the average conversion rates based on the new page provided. (based on the **p_old = p_new null** hypothesis).

## Conclusions 

Based on the tests we ran on the data provided, here are the conclusions:

- The old page should be kept as there was not enough statistically significant evidence to reject the null hyopthesis in the A/B test and z test done.
- The regression models created conclude that the new page variable and other factors such as countries are not statiscally significant in predicting the likelihood of changes in the average conversion rates.
