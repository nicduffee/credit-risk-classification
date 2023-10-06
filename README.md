# Credit Risk Classification

Supervised Machine Learning, Python, Pandas

## Overview of the Analysis

Develop a Machine Learning algorithim analysing historic lending data to help identify high-risk loans.

The dataset has the following features:
- loan size
- interest rate
- borrower income
- debt to income percentage
- number of accounts
- any derogatory marks
- total debt size

Given the actual loan status of each loan, the algorithim can be trained on a training set, split from the provided dataset. It can then be tested on a test set of data using a `LogisticRegression` model from scikit-learn to predict wether or not the loan is high risk.

## Results

### Machine Learning Model 1:

Accurary: 95% </br>
Percision: 99% Low Risk, 91% High Risk </br>
Recall: 100% Low Risk, 85% High Risk </br>

### Machine Learning Model 2:
(Using a random over sampler)

Accurary: 99% </br>
Percision: 99% Low Risk, 99% High Risk </br>
Recall: 100% Low Risk, 84% High Risk </br>

## Summary
Model 2 would be my recommendation for model as it correctly labels both healthy and high-risk loans with 99% accurary (precision score). however the limitations must be taken into account that it only identifies 84% of the high-risk loans, meaning it misses 16% of the high-risk loans (recall score)
