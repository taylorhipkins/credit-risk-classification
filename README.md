# credit-risk-classification
This repository contains all necessary files for the Module 20 challenge, credit risk classification.

## Overview of the Analysis 
The purpose of this analysis was to develop and evaluate machine learning models for credit risk assessment in loan applications. The primary goal was to predict whether a loan is likely to be healthy (0) or high-risk (1) based on various financial indicators provided in the dataset.
The target variable for prediction was the loan_status column, where a value of 0 indicated a healthy loan and a value of 1 indicated a high-risk loan.
To gain insights into the data, I initially explored the distribution of the target variable using value_counts() to understand the balance between healthy and high-risk loans. This step helped to identify any class imbalances that might affect the model's performance.
The machine learning process involved several stages:
Data Preprocessing: This stage involved cleaning the data, handling missing values, encoding categorical variables, and scaling numerical features if necessary to prepare the data for modeling.
Feature Selection/Engineering: I examined the correlation between features and the target variable to select the most relevant features for the model. Additionally, I explored the possibility of creating new features that might enhance predictive performance.
Model Selection: For this analysis, I employed logistic regression as the primary algorithm due to its interpretability and suitability for binary classification tasks. 
Model Training and Evaluation: I split the data into training and testing sets using train_test_split() and trained the logistic regression model on the training data. Following that, I evaluated the model's performance on the testing data using metrics such as accuracy, precision, recall, and F1-score. Additionally, I generated a confusion matrix and classification report to assess the model's ability to predict both healthy and high-risk loans accurately.

## Results
Precision (Class 0 - Healthy Loan):
Precision score of 1.00 means that when the model predicts a loan as healthy, it is correct 100% of the time.
Recall score of 0.99 indicates that the model correctly identifies 99% of the healthy loans out of all actual healthy loans.
F1-score of 1.00 represents the harmonic mean of precision and recall for class 0.
Precision (Class 1 - High-Risk Loan):
Precision score of 0.85 indicates that when the model predicts a loan as high-risk, it is correct 85% of the time.
Recall score of 0.91 suggests that the model correctly identifies 91% of the high-risk loans out of all actual high-risk loans.
F1-score of 0.88 represents the harmonic mean of precision and recall for class 1.
Accuracy:
The overall accuracy score of 0.99 indicates that the model correctly predicts 99% of the loans' statuses (either healthy or high-risk) overall.
Recall (Sensitivity) (Class 0 - Healthy Loan):
Recall score of 0.99 indicates that the model correctly identifies 99% of the healthy loans out of all actual healthy loans. This means it has a high sensitivity to detecting healthy loans.
Recall (Sensitivity) (Class 1 - High-Risk Loan):
Recall score of 0.91 suggests that the model correctly identifies 91% of the high-risk loans out of all actual high-risk loans. This indicates that the model has a relatively good sensitivity in detecting high-risk loans, though it may miss some.

## Summary
The machine learning model developed for credit risk assessment in loan applications performed exceptionally well overall, demonstrating high accuracy and balanced performance across both healthy and high-risk loan categories.
Performance Comparison:
The model achieved an accuracy score of 0.99, indicating that it correctly predicts 99% of loan statuses overall.
In terms of precision, the model achieved a perfect precision score of 1.00 for healthy loans (class 0), implying that it correctly identifies all healthy loans when predicting them. For high-risk loans (class 1), the precision score is 0.85, indicating that it correctly identifies 85% of high-risk loans out of all predicted high-risk loans.
Similarly, the recall (sensitivity) scores reflect the model's ability to capture instances of both healthy and high-risk loans. The recall score for healthy loans is 0.99, suggesting that the model correctly identifies 99% of actual healthy loans. For high-risk loans, the recall score is 0.91, indicating that it correctly identifies 91% of actual high-risk loans.
The F1-scores, which are the harmonic mean of precision and recall, further validate the balanced performance of the model, with an F1-score of 1.00 for healthy loans and 0.88 for high-risk loans.
Consideration of Problem Importance:
In many cases, there might be a higher emphasis on accurately predicting high-risk loans (class 1) to avoid potential financial risks associated with defaulting loans. However, the balanced performance of the model across both classes indicates its effectiveness in addressing the needs of both objectives.
Recommendation: Based on the analysis, the logistic regression model performs exceptionally well for credit risk assessment in loan applications. Its high accuracy, precision, and recall scores indicate that it effectively distinguishes between healthy and high-risk loans. Therefore, I recommend utilizing this logistic regression model for credit risk assessment purposes, as it provides valuable insights to lending institutions for making informed decisions regarding loan approvals and risk management strategies.


## Data Aquisition
lending_data.csv located in resources folder

## Languages Used
python
