# Credit Risk Analysis Report
# Overview of the Analysis
The primary purpose of this analysis was to assess the creditworthiness of borrowers using historical lending data from a peer-to-peer lending service. The objective was to predict the likelihood of loan defaults, classifying loans as either healthy (0) or high-risk (1) based on various borrower characteristics and loan attributes.

The dataset contained information on past loans, including features such as loan amount, interest rate, borrower income, and loan purpose. The target variable was the loan_status, where a value of 0 indicates a healthy loan, and a value of 1 indicates a high-risk loan.

To better understand the dataset, the following distribution of the target variable was observed:

Healthy loans (0): 15,001 (approximately 96.9%)
High-risk loans (1): 507 (approximately 3.1%)
The analysis followed a structured machine learning process:

## Data Preparation: The dataset was read into a Pandas DataFrame, and the target variable was separated from the features.
## Data Splitting: The dataset was divided into training and testing sets to ensure a robust evaluation of model performance.
## Model Training: A Logistic Regression model was fitted to the training data.
## Model Evaluation: The model's performance was evaluated using metrics such as accuracy, precision, recall, and a confusion matrix.
### Results
Logistic Regression Model:
Accuracy: 99%
Precision (Healthy Loan): 100%
Recall (Healthy Loan): 100%
Precision (High-Risk Loan): 86%
Recall (High-Risk Loan): 91%
The results indicate that the Logistic Regression model performed exceptionally well in predicting healthy loans, achieving perfect precision and recall scores. For high-risk loans, while the model demonstrated good performance, there was a slight drop in precision and recall, suggesting some room for improvement in accurately classifying this category.

# Summary
Based on the analysis, the Logistic Regression model is recommended for use in predicting borrower creditworthiness. It shows a high level of accuracy overall, particularly in identifying healthy loans, which is crucial for minimizing financial risk for the lending company.

While the model effectively predicts healthy loans, the accuracy in identifying high-risk loans is slightly lower. This discrepancy highlights the need for ongoing monitoring and potential adjustments to enhance model performance further, especially since accurately identifying high-risk loans is critical for managing loan defaults.

Given the nature of the financial industry, it is essential to balance the importance of predicting both healthy and high-risk loans. In this case, it may be more vital to reduce the number of false negatives (misclassifying high-risk loans as healthy) to mitigate potential financial losses.

