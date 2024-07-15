# Employee Attrition Prediction Model

## Overview
Employee attrition is a significant challenge for organizations, impacting their operational efficiency, financial health, and overall productivity. High turnover rates can lead to increased recruitment and training costs, loss of organizational knowledge, and decreased employee morale. The primary goal of this project is to develop a predictive model that accurately identifies employees who are likely to leave the company. By leveraging this model, organizations can proactively address the factors contributing to attrition, implement targeted retention strategies, and ultimately reduce turnover rates. This model can provide valuable insights to Human Resource Managers, Organizational Leaders, and Business Strategists, helping them to enhance employee engagement, improve workplace satisfaction, and optimize workforce management strategies.

## Data Source
The data used in this project comes from the HR Employee Attrition dataset available on Kaggle. This dataset contains comprehensive information on various employee attributes, both numerical and categorical, that are relevant for predicting attrition. The dataset includes 1470 records and 35 features, making it sufficiently large and diverse for building robust predictive models.

## Stakeholders
**Human Resource Managers:** Can use the model to identify at-risk employees and implement retention strategies.
**Organizational Leaders:** Can leverage insights from the model to improve employee engagement and satisfaction.
**Business Strategists:** Can use the predictive insights to plan and execute better workforce management strategies.

## Summary of Data Science Steps
1. Data Exploration

-Inspected data types, unique values, and distribution of the target variable.

2. Data Processing

-One-hot encoded categorical variables and scaled numerical ones.

3. Model Training: Logistic Regression
   
-Two logistic regression models were trained and evaluated using cross-validation.

-Iterative functions were defined and used to find the best parameters.

4. Model Training: Decision Trees

-Multiple decision tree models were trained and evaluated.

-Iterative functions were defined and used to find the best parameters.

5. Model Evaluation

-The final model was evaluated on the holdout data.
