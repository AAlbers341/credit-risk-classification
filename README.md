## credit-risk-classification

## Overview of the Analysis

The primary objective of this analysis is to employ Logistic Regression, a powerful regression analysis technique tailored for predicting the probability of a binary outcome using multiple predictor variables. Specifically, this study harnesses lending data containing essential financial metrics such as 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income', 'num_of_accounts', 'derogatory_marks', and 'loan_status'. The overarching goal is to assess the creditworthiness of borrowers by accurately predicting the likelihood of a borrower being categorized based on their financial attributes.

The process for the logistic regression analysis over lending data is as follows:
1.) Load in data for 'lending_data.csv'
    a.) Identify our target variable vs features
    b.) Split the data into training and testing dataset by using 'train_test_split' from sklearn.model_selection library

2.) Create a Logistic Regression Model
    a.) From sklearn.linear_model, import Logistic Regression package to instantiate the model 
    b.) Fit the model using our trained features and labels
    c.) Make prediction using the testing data 

3.) Measure the model evaluation by using the classification report
    a.) Identify how the model is performing by utilizing precision, recall and F1-scores


## Results

Machine Learning Model 1:
Accurary score: 99%
    ♦ Healthy Loan(0)
        - Precision: 100%
        - Recall:    100%
        - F1-score:  100%

    ♦ High-Risk Loan(1)
        - Precision:  94%
        - Recall:     89%
        - F1-score:   88%


## Summary

Overall, the classification report performs very well, with high precision, recall and F1-score for both classes. The model is very good at predicting healthy loans; however, predicting high-risk loans can lead to some potential risk. 

For healthy loans, the model predicts 100% precision, recall and F1-score which indicates that all instances classified as 'healthy loans' were actually 'healthy loans', all 'healthy loans' were correctly identified and there is a perfect balance between precision and recall.
For high-risk loans, the model's precision is 87% which indicates that 87% of instances classified as 'high-risk loans' were actually 'high-risk loans'. For recall for high-risk loans, the recall is 89% with indicates that 89% of 'high-risk loans' instances were correctly identified. Lastly, with a F1-score of 88% for high-risk score, there is some variability between the balance of precision and recall. 
