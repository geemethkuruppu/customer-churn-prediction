# Customer Churn Prediction

This machine learning project aims to predict customer churn using various classification techniques, primarily focusing on **Logistic Regression**. The dataset is based on a telecom company's customer data.

---

# Project Overview

- **Goal:** Predict whether a customer will churn (leave the service).
- **Model:** Logistic Regression
- **Handling Imbalance:** SMOTE (Synthetic Minority Oversampling Technique)
- **Feature Scaling:** Standardization using `StandardScaler`
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC

---

## Dataset

The dataset contains **7043 rows** and **21 columns**, including:
- **Categorical**: gender, Partner, Dependents, etc.
- **Numerical**: tenure, MonthlyCharges, TotalCharges
- **Target**: `Churn` (Yes/No)

---

# Exploratory Data Analysis (EDA)

- Checked for missing and duplicate values.
- Visualized distribution of categorical variables using `seaborn`.
- Detected class imbalance in `Churn`.
- Investigated correlation among numeric features.

---

## Data Preprocessing

- Removed customerID column (not useful).
- Handled missing values in `TotalCharges` column.
- Converted `TotalCharges` to numeric.
- One-hot encoded categorical features.
- Standardized numerical features (`tenure`, `MonthlyCharges`, `TotalCharges`).

---

# Handling Class Imbalance

- Used `SMOTE` to balance the dataset:
  - Before: ~73% No churn, ~27% Yes churn
  - After: 50/50 balance in training data

---

# Model: Logistic Regression

- Used Logistic Regression with:
  - Scaled features
  - Performance evaluation

---

# Evaluation Metrics

- **Accuracy:** 78%
- **Precision, Recall, F1-score:** Evaluated using classification report
- **Confusion Matrix**: For understanding false positives/negatives

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/geemethkuruppu/customer-churn-prediction.git
   cd customer-churn-prediction
