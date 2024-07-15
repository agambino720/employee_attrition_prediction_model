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
**1. Data Exploration**

   -Inspected data types, unique values, and distribution of the target variable.

**2. Data Processing**

   -One-hot encoded categorical variables and scaled numerical ones.

**3. Model Training: Logistic Regression**
   
   -Two logistic regression models were trained and evaluated using cross-validation.

   -Iterative functions were defined and used to find the best parameters.

**4. Model Training: Decision Trees**

   -Multiple decision tree models were trained and evaluated.

   -Iterative functions were defined and used to find the best parameters.

**5. Model Evaluation**

   -The final model was evaluated on the holdout data.

## Model Performance on Holdout Data

### Metrics
The final model used in this analysis is a class weight adjusted decision tree, which was carefully tuned to enhance its performance in predicting employee attrition. This model was chosen because it provided the best balance between identifying employees who might leave and maintaining overall prediction accuracy. The key metrics for this model on the holdout data included an accuracy of 68.03%, with a precision of 0.89, recall of 0.70, and F1-score of 0.79 for non-attrition cases. For predicting attrition, the model achieved a precision of 0.26, recall of 0.55, and F1-score of 0.36. Cross-validation further supported these findings, with a mean recall of 0.41 and a standard deviation of 0.16.

### Implications of Metrics
This model correctly identified approximately 55% of the actual attrition cases, allowing the business to take proactive measures for more than half of the employees at risk of leaving. However, the model had a precision of 26% for attrition, meaning many predicted attrition cases were not actual attrition cases. The model also misclassified 29.56% (73 out of 247) of non-attrition cases as attrition cases, potentially leading to unnecessary interventions. While there is room for improvement, this model provides a starting point for addressing employee attrition by correctly identifying a significant portion of at-risk employees, which can help in designing targeted retention strategies.

## Justification of Metrics and Model Evaluation
The choice of recall as a key metric is justified in the context of the real-world problem of employee attrition. The consequences of failing to identify at-risk employees can be severe, including increased recruitment and training costs, loss of organizational knowledge, and decreased productivity. By focusing on recall, the model ensures that the business can take timely actions to retain employees, thereby mitigating these negative impacts. The final model, identified based on its performance on the chosen metrics with validation data, was evaluated using holdout data. The performance metrics on the test data reaffirmed the model's effectiveness in identifying attrition cases while maintaining an acceptable level of overall accuracy.

## Implications for Stakeholders
For stakeholders, the implications of using this model are substantial. By accurately identifying a significant proportion of employees who are at risk of leaving, the business can implement targeted retention strategies, such as employee engagement programs, career development opportunities, and improved working conditions. This proactive approach can reduce turnover costs, maintain workforce stability, and enhance overall employee satisfaction. In the long run, this predictive capability allows the business to foster a more stable and committed workforce, leading to better organizational performance and competitive advantage. By focusing on recall, the business ensures that it is better prepared to handle potential attrition and can take steps to mitigate its impact, thereby supporting a more sustainable and efficient organizational environment.

## Repository Structure
**README.md:** This file provides an overview of the project and instructions for navigating the repository.

**employee_attrition_project.ipynb:** Contains the Jupyter Notebook with all the code, model iterations, and model evaluation related to the project.

**.gitignore:** Specifies files and directories to be ignored by Git.

**data:** Directory containing the HR-Employee-Attrition.csv dataset used for the analysis.

## Links
**Presentation:** 
https://docs.google.com/presentation/d/1574tq9Vk5slwx3Pt093wnDFCVHATwoRIMk7LDILbz2A/edit?usp=sharing

**Data Source:**
https://www.kaggle.com/datasets/itssuru/hr-employee-attrition/data
