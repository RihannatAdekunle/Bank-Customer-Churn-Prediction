# Bank Customer Churn Prediction

This project explores multiple machine learning models to predict customer churn in a banking context. By analyzing customer demographics, account activity, and historical data, we aim to identify customers at risk of leaving the bank, providing insights for targeted retention strategies.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Project Structure](#project-structure)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Evaluation](#evaluation)
- [Results and Insights](#results-and-insights)
- [Conclusion](#conclusion)
- [Future Work](#future-work)

---

## Project Overview
Customer churn prediction is essential for banks to reduce attrition rates. This project uses three machine learning models to predict customer churn, leveraging customer data like age, balance, and activity level. The ultimate goal is to provide actionable insights that help retain valuable customers.

## Objectives
- Clean and preprocess data to ensure consistency and quality.
- Perform exploratory data analysis (EDA) to identify key patterns and trends.
- Build and evaluate multiple machine learning models to classify customers as "churn" or "not churn."
- Select the best-performing model for practical use.

## Dataset
The dataset includes several customer-related features:
- **CustomerID**: Unique identifier
- **Surname**: Customer's last name
- **Geography**: Country of residence
- **Gender**: Gender of the customer
- **Age**: Customer's age
- **Balance**: Account balance
- **IsActiveMember**: Binary indicator of active status
- **Exited**: Target variable indicating churn (1 for churned, 0 for retained)

## Technologies Used
- **Python** (Libraries: `pandas`, `scikit-learn`, `numpy`, `matplotlib`, `seaborn`)
- **Jupyter Notebook**

## Setup and Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/RihannatAdekunle/Bank_Customer_Churn_Prediction.git
   cd Bank_Customer_Churn_Prediction

 ## Project Structure
```plaintext
Bank_Customer_Churn_Prediction/
├── Bank_customer_churn.ipynb      # Jupyter notebook with full code
├── README.md                      # Project documentation
├── requirements.txt               # Dependencies for the project

