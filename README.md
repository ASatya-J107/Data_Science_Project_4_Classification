# Customer Churn Prediction

Predicting customer churn is crucial for businesses, as retaining existing customers is often more cost-effective than acquiring new ones. This repository contains Python code for predicting customer churn in a telecommunications company. The code follows a step-by-step process, including data import, preprocessing, exploratory data analysis (EDA), model selection, and evaluation.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Import](#data-import)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Feature Engineering](#feature-engineering)
6. [Model Selection](#model-selection)
7. [Model Evaluation](#model-evaluation)
8. [Predicting Customer Churn for New Data](#predicting-customer-churn-for-new-data)
9. [Conclusion](#conclusion)
10. [Usage](#usage)
11. [License](#license)

## Introduction
Customer churn, also known as customer attrition, occurs when customers discontinue using a company's services or products. Predicting and preventing churn is essential for maintaining a healthy customer base and revenue stream. In this project, we build a machine learning model to predict customer churn based on historical customer data.

## Data Import
The code begins by importing relevant Python libraries for data analysis, preprocessing, modeling, and evaluation. It then imports the dataset, which presumably contains customer information and churn labels.

## Data Preprocessing
Data preprocessing is a crucial step in any machine learning project. This section includes the following sub-steps:
- **Evaluate Data Structure:** Provides an overview of the dataset, including the first few rows, column names, basic statistics, data types, and information about missing values.
- **Check Target Variable Distribution:** Examines the distribution of the target variable "Churn" to address potential class imbalance.
- **Clean the Dataset:** Handles missing values and converts the "TotalCharges" column to a numeric data type.
- **Label Encode Binary Data:** Encodes binary categorical data such as "gender," "Partner," "Dependents," "PhoneService," "PaperlessBilling," and "Churn."

## Exploratory Data Analysis (EDA)
Exploratory data analysis is essential for understanding the dataset and identifying patterns. This section includes the following:
- **Plot Histogram of Numeric Columns:** Visualizes histograms for numerical columns like age, tenure, monthly charges, etc.
- **Analyze Distribution of Key Categorical Variables:** Analyzes and plots the distribution of categorical variables such as contract type, payment method, and various label-encoded variables.
- **Analyze Churn Rate by Categorical Variables:** Examines churn rates based on contract type and payment method.

## Feature Engineering
Feature engineering involves creating new features or transforming existing ones to improve model performance. While this project focuses more on model selection and evaluation, feature engineering can be extended based on domain knowledge and dataset-specific insights.

## Model Selection
To predict customer churn, various classification algorithms are considered:
- Logistic Regression
- Support Vector Classifier (SVC)
- Kernel SVM
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
- Decision Tree Classifier
- Random Forest Classifier

Each model is evaluated using cross-validation, and performance metrics such as accuracy, precision, recall, F1-score, F2-score, and ROC AUC are recorded.

## Model Evaluation
Model performance is visualized and compared using boxplots to highlight variations in accuracy across different classification algorithms. Specific models (Logistic Regression, Decision Tree, and Random Forest) are fitted and evaluated in terms of accuracy, precision, recall, F1-score, F2-score, and ROC AUC. Results are sorted based on precision, recall, and F2-score to prioritize models that minimize false negatives.

## Predicting Customer Churn for New Data
The code demonstrates how to predict customer churn for new data. It preprocesses new data, scales it using the same scaler as the training data, and uses the trained Logistic Regression model to make predictions.

## Conclusion
Predicting customer churn is a critical task for businesses aiming to retain their customer base. This project provides a comprehensive example of how to build, evaluate, and deploy a machine learning model for churn prediction. Customization and further feature engineering can enhance model performance.
