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
   git clone https://github.com/yourusername/Bank_Customer_Churn_Prediction.git
   cd Bank_Customer_Churn_Prediction

 ## Project Structure
```plaintext
Bank_Customer_Churn_Prediction/
├── Bank_customer_churn.ipynb      # Jupyter notebook with full code
├── README.md                      # Project documentation
├── requirements.txt               # Dependencies for the project

## Data Preprocessing
The data preprocessing phase is crucial for ensuring data quality and consistency. The steps taken to preprocess the data are as follows:

1. **Data Cleaning**:
   - **Dropped Irrelevant Columns**: Removed `CustomerID` and `Surname` since they don't contribute to the prediction of churn and may introduce noise.
   - **Missing Values Handling**: Verified there were no missing values; otherwise, missing values would be handled through imputation or removal.

2. **Encoding Categorical Variables**:
   - **One-Hot Encoding**: Applied one-hot encoding on categorical columns such as `Geography` and `Gender` to convert these categories into numerical values, enabling the model to process them effectively.

3. **Feature Scaling**:
   - **Standardization with StandardScaler**: To ensure that all features contribute equally to the model, we applied `StandardScaler` to numerical columns (e.g., `Balance`, `Age`, `CreditScore`). This process scales the values to a mean of 0 and standard deviation of 1, helping improve model convergence and performance.

Each of these preprocessing steps was applied consistently across the training and test datasets to maintain data integrity for accurate model evaluation.

## Model Building
This project explores three machine learning models to predict customer churn. Each model has unique strengths, allowing for a comparison of performance and interpretability. The models used are:

1. **Logistic Regression**:
   - Chosen for its simplicity and effectiveness in binary classification tasks.
   - Provides interpretability through feature coefficients, offering insights into which variables contribute most to the likelihood of customer churn.

2. **Linear Regression**:
   - Adapted for classification by applying a threshold on predicted values, transforming them into binary outputs for churn prediction.
   - Used to compare against other models, even though it is traditionally a regression model.

3. **Decision Tree Classifier**:
   - A tree-based model that segments data based on feature importance, creating splits that are easily interpretable.
   - Suitable for understanding which features most influence churn and helpful for visualizing decision paths.

### Training and Prediction
- **Training**: Each model was trained on a preprocessed training dataset. During this phase:
  - The data was split into training and testing sets to evaluate model performance.
  - A `fit` function was called to train the models on the training set, allowing them to learn patterns related to churn.
  
- **Prediction**: Predictions were generated for the test dataset using each trained model. The predictions represent each customer’s likelihood of churn based on the model’s analysis.

The training and prediction processes were repeated for all three models, allowing a comparative analysis of performance metrics like accuracy, precision, recall, and F1 score.

---




