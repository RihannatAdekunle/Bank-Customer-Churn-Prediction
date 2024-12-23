# Bank Customer Churn Prediction

## Table of Contents
- [Introduction](#introduction)
- [Dataset Overview](#dataset-overview)
- [Methodology](#methodology)
- [Model Performance Comparison](#model-performance-comparison)
- [Insights](#insights)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

---

## Introduction
This report presents an in-depth analysis of customer churn prediction for a bank. Key findings reveal that older, inactive customers and those in Spain are more likely to churn. The Logisitic Regression model demonstrated the best performance, with 79% accuracy and actionable insights derived from feature importance analysis. Recommendations focus on retention strategies targeting at-risk groups. This study leverages customer demographic and account activity data to predict churn using machine learning models. The objective is to reduce attrition rates and guide retention strategies.

---

## Dataset Overview
The dataset contains 14 features including customer demographics, account activity, and the target variable, `Exited`, which indicates customer churn (1 = churned, 0 = retained). The features include:
- `CustomerId`: Unique identifier
- `CreditScore`: Customer's credit score
- `Geography`: Country of residence
- `Gender`: Gender of the customer
- `Age`: Customer's age
- `Balance`: Account balance
- `IsActiveMember`: Indicates if the customer is active
- `EstimatedSalary`: Customer's estimated salary

---

## Methodology
The analysis involves the following steps:

1. **Data Preprocessing**:  
   - Handling missing values, encoding categorical features, and scaling numerical variables.  
   - Key actions:
     - No missing values were detected.
     - Categorical variables (`Geography`, `Gender`) were encoded.
     - Numerical features were scaled using `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**:  
   - Identifying patterns, correlations, and trends.  
   - Key observations:
     - Churn is higher among female customers.
     - Customers from Spain exhibited higher churn rates compared to France and Germany.
     - Older customers are more likely to churn.
     - Inactive members and those with zero balance have elevated churn rates.

3. **Model Training**:  
   - Using Logistic Regression, Decision Tree, and Linear Regression models to predict churn.

4. **Model Evaluation**:  
   - Comparing models based on metrics like accuracy, precision, recall, and AUC.

---

## Model Performance Comparison

| Model              | Accuracy | Precision | Recall | F1-Score | AUC  |
|---------------------|----------|-----------|--------|----------|------|
| Logistic Regression | 79%      | 0.63      | 0.79   | 0.70     | 0.78 |
| Decision Tree       | 77%      | 0.77      | 0.78   | 0.77     | 0.83 |
| Linear Regression  | 14%      | 0.20     | 0.13   | 0.13     | 0.13 |

---

## Insights
1. **Age**:
   - Older customers show higher churn rates, potentially due to reduced engagement with banking services or dissatisfaction with current offerings.

2. **Activity Level**:
   - Inactive members (`IsActiveMember=0`) have significantly higher churn rates, highlighting the importance of customer engagement.

3. **Gender and Balance**:
   - Female customers exhibit higher churn rates, suggesting differences in banking needs or service satisfaction compared to male customers.
   - Customers with zero balance are at higher risk, reflecting dissatisfaction or lack of financial activity.

4. **Geography**:
   - Spanish customers are more likely to churn, emphasizing a need for localized strategies.

---

## Recommendations
1. **Target Older Customers**:
   - Develop customized products and services tailored for older customers, such as retirement accounts or loyalty programs.
   - Provide personalized communication and offers to demonstrate value.

2. **Re-engage Inactive Members**:
   - Launch proactive outreach campaigns, including reminders, exclusive offers, or incentives.
   - Implement rewards programs that incentivize consistent use of banking services.

3. **Focus on Female Customers**:
   - Conduct further analysis to understand their needs and expectations.
   - Develop marketing campaigns and customer service initiatives tailored to this demographic.

4. **Address Zero-Balance Accounts**:
   - Encourage account activity through targeted offers and incentives.

5. **Localized Campaigns for Spain**:
   - Design campaigns addressing specific pain points or preferences in Spain.
   - Analyze feedback from Spanish customers to identify dissatisfaction sources and prioritize solutions.

---

## Conclusion
This analysis demonstrates the importance of understanding customer behavior to address churn effectively. Logisitc Regression emerged as the best-performing model, offering the most accurate predictions and actionable insights. By targeting at-risk customer segments—older, inactive, female customers—banks can develop data-driven retention strategies.
