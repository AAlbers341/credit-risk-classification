## credit-risk-classification

### Overview of the Analysis

The primary objective of this analysis is to employ Logistic Regression, a powerful regression analysis technique tailored for predicting the probability of a binary outcome using multiple predictor variables. Specifically, this study harnesses lending data containing essential financial metrics such as 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income', 'num_of_accounts', 'derogatory_marks', and 'loan_status'. The overarching goal is to assess the creditworthiness of borrowers by accurately predicting the likelihood of a borrower being categorized based on their financial attributes.

#### Process for the Logistic Regression Analysis:
1. **Load Data**: Load the 'lending_data.csv' dataset.
    - Identify target variable and features.
    - Split the data into training and testing datasets using 'train_test_split' from the sklearn.model_selection library.

2. **Create Logistic Regression Model**:
    - Instantiate the Logistic Regression model from sklearn.linear_model.
    - Fit the model using the training features and labels.
    - Make predictions using the testing data.

3. **Model Evaluation**:
    - Utilize classification report to assess model performance, focusing on precision, recall, and F1-scores.

### Results

**Machine Learning Model 1:**
- Accuracy score: 99%
    - **Healthy Loan (0)**
        - Precision: 100%
        - Recall: 100%
        - F1-score: 100%
    - **High-Risk Loan (1)**
        - Precision: 94%
        - Recall: 89%
        - F1-score: 88%

### Summary

Overall, the classification report demonstrates excellent performance, with high precision, recall, and F1-scores for both classes. The model effectively predicts healthy loans, achieving perfect precision, recall, and F1-score. However, there is a slight variability in predicting high-risk loans, indicating potential risk in misclassification.

- **Healthy Loans**: The model exhibits perfect precision, recall, and F1-score, signifying accurate identification of all healthy loan instances with a perfect balance between precision and recall.
- **High-Risk Loans**: Although the precision is 87%, indicating that 87% of high-risk loan classifications are accurate, there is room for improvement in recall (89%) and F1-score (88%), indicating some variability in the balance between precision and recall.