# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Purpose of the analysis: to train and evaluate Logistic Regression models to correctly identify credtworthiness of borrowers.
* Financial information that the data related to: Lending data on customers: Loan size, interest rate, borrower income, debt to income ratio, number of accounts, deragatory remarks, total debt and loan status
    *What we needed to predict: loan status (whether the loan was healthy or high-risk)
* Stages of the machine learning process:
  1. Counting rows that had score 0 (healthy) vs. score 1 (high-risk)
  2. Train-test split
* Methods Used: Logistic regression, oversampling

## Results

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.9520479254722232
  * Overall Accuracy: 99%
  * Precision: 100% for healthy loans, 85% for high-risk loans
  * Recall: 99% for healthy loans, 91% for high-risk loans
  
                 precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384



* Machine Learning Model 2:
  * Balanced Accuracy Score: 0.9936781215845847
  * Overall Accuracy: 99%
  * Precision: 100% for healthy loans, 84% for high-risk loans
  * Recall: 99% for healthy loans, 99% for high-risk loans
  
  
                 precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

## Summary

Model 2 (the oversampled logitstic model) seems to perform slightly better than Model 1 (the original logistic model). Model 2 has less variation between f1-score classification categories (0 for healthy loan and 1 for high-risk loan), and stronger recall compared to model 1. If one had to pick between the two models, I would recommend using model 2. However, a better model may still exist. 

