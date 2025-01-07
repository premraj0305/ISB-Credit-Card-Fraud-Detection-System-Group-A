# Credit Card Fraud Detection

#Team members
      Prarthana G                      
      Prem Raj P
      Shailesh KR                      
      Ashvini Kumar
      Sri Lalitha B                        
      Mansi Ranjan Gupta
      Oleti Chandini


## Overview
This project aims to classify credit card transactions as fraudulent or non-fraudulent using machine learning techniques. The dataset used for this project is the "Credit Card Fraud Detection" dataset from Kaggle, which contains anonymized features and transaction information.

## Problem Statement
The objective is to build a robust model capable of identifying fraudulent transactions to mitigate risks and improve financial security.

## Dataset
- **Source**: Kaggle - [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Description**: The dataset includes 284,807 transactions with 31 features (28 anonymized features, time, amount, and class).
- **Class Distribution**:
  - 0: Non-fraudulent transactions (majority class)
  - 1: Fraudulent transactions (minority class)

## Dataset Overview
- **Total Data**: 555,458
- **Total Rows in Dataset**: 41,683
- **Columns**: 31
- **Class Distribution in Raw Data**:
  - Non-Fraudulent Transactions: 41,574
  - Fraudulent Transactions: 108

## Dependencies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- imbalanced-learn
- XGBoost
- CatBoost
  
## Steps Followed

### 1. Data Preprocessing
- Checked for null values and data consistency.
- Scaled numerical features using `RobustScaler`.
- Balanced the class distribution using SMOTE (Synthetic Minority Oversampling Technique).

### 2. Exploratory Data Analysis (EDA)
- Analyzed the distribution of fraudulent and non-fraudulent transactions.
- Visualized transaction amount trends and time-based patterns.
- Applied standardization to numerical features.
- Addressed the class imbalance using oversampling techniques (e.g., SMOTE).
  
- **Correlation Heatmap**:
  - Analyzed correlations between features and the target variable.
  - Identified features most related to fraudulent transactions.
- **Recursive Feature Elimination (RFE)**:
  - Iteratively removed less significant features based on model performance.
  - Focused on reducing redundancy and improving model interpretability.

### 3. Model Development
- Implemented various machine learning models:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting (XGBoost)
  - Neural Networks
  - CatBoost
- Evaluated performance using metrics like accuracy, precision, recall, F1-score, and AUC-ROC.

### 4. Model Evaluation
- Used cross-validation to assess model performance.
- Compared metrics to identify the best-performing model.
- **Best Performing Model**: CatBoost with an accuracy of 99.95%

## Results
- Achieved high precision and recall on the minority (fraudulent) class.
- Selected the best-performing model based on AUC-ROC and F1-score.
- Fraudulent transactions are sparse, but the models effectively classified them.

## Conclusion
This project successfully demonstrates the application of machine learning techniques to detect fraudulent transactions in credit card data. By addressing challenges such as class imbalance and feature anonymization, the developed models achieved high accuracy and reliability. The insights gained can be extended to real-world systems to enhance financial security and mitigate fraud risks.
