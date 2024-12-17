# Credit Card Customer Attrition Prediction

## Abstract
In the era of digital transactions, credit card usage has surged, making customer retention crucial for banks to sustain profitability. This project focuses on predicting credit card customer churn using machine learning models. Four models—Logistic Regression, Decision Tree, Random Forest, and Light GBM—are applied to a dataset containing over 10,000 data points and 20 features.

## Introduction
In today's competitive market, credit cards are vital for a bank's profitability, making customer turnover a critical concern. Higher retention rates correlate with increased profits. Leveraging machine learning models on large customer datasets enables proactive churn prediction, allowing banks to enhance services or offer enticing discounts to retain customers.

## Method
- **Logistic Regression:** Models the probability of a binary outcome using a sigmoid function, handling nonlinear correlations.
- **Decision Tree:** Utilizes a tree structure to segment data into subsets, making decisions based on features. Handles uncertainty using entropy and information gain.
- **Random Forest:** An ensemble learning technique combining multiple decision trees, mitigating variance and bias by random sampling and feature subsets.
- **Light GBM:** A gradient boosting decision tree variant known for its computational efficiency, parallel learning, and memory usage.

## Evaluation Criteria
Model performance is evaluated using confusion matrices and metrics such as accuracy, precision, recall, and F1 score.

## Data
The dataset, sourced from Kaggle, comprises information on 10,000 credit card holders with 21 variables including demographics, financial attributes, and transaction history.

## Exploratory Data Analysis
EDA involves handling missing values, outliers, and visualizing feature distributions and relationships with the target variable (attrition flag).

## Data Cleaning
Missing values are imputed, and unwanted columns are dropped. Categorical features are encoded using label encoding and one-hot encoding.

## Data Preparation
The dataset is divided into train, validation, and test sets using stratified sampling. Feature scaling and resampling techniques (over and under-sampling) are applied.

## Modelling and Explanation
Four models are tested and evaluated based on recall and ROC-AUC scores. Hyperparameter tuning is performed using RandomizedSearchCV.

## Conclusion
The Light GBM model trained on the under-sampled dataset performs best. Important features influencing attrition include transaction-related metrics and customer engagement indicators.

## Future Scope
Potential areas for further exploration include utilizing more sophisticated algorithms, expanding the dataset, and employing advanced ensembling techniques.
