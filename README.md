# Customer Churn Prediction

## Project Overview

This project predicts whether a customer will leave the bank or stay using Machine Learning algorithms.

The dataset contains customer information such as:

* Credit Score
* Geography
* Gender
* Age
* Balance
* Number of Products
* Active Member Status
* Estimated Salary
* etc.

The target column is:

* `Exited`

  * `0` → Customer Stayed
  * `1` → Customer Left

This is a Binary Classification Machine Learning project.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib

---

# Machine Learning Models Used

* Logistic Regression
* Random Forest Classifier

---

# Project Workflow

```text
Load Dataset
    ↓
Data Preprocessing
    ↓
Handle Categorical Features
    ↓
Train Test Split
    ↓
Feature Scaling
    ↓
Train Model
    ↓
Prediction
    ↓
Model Evaluation
    ↓
Save Model
```

---

# Dataset Features

| Feature         | Description             |
| --------------- | ----------------------- |
| CreditScore     | Customer credit score   |
| Geography       | Customer country        |
| Gender          | Male/Female             |
| Age             | Customer age            |
| Tenure          | Years with bank         |
| Balance         | Bank balance            |
| NumOfProducts   | Number of bank products |
| HasCrCard       | Credit card status      |
| IsActiveMember  | Active member status    |
| EstimatedSalary | Estimated salary        |
| Exited          | Target column           |

---

# Data Preprocessing

The following preprocessing steps were performed:

* Removed unnecessary columns:

  * RowNumber
  * CustomerId
  * Surname

* Applied One Hot Encoding on:

  * Gender
  * Geography

* Applied Feature Scaling using StandardScaler

---

# Model Evaluation Metrics

The following metrics were used:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1 Score

---

# Installation

## Clone Repository

```bash
git clone <your-github-repo-link>
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Run Project

```bash
python churn_prediction.py
```

---

# Project Structure

```text
Customer-Churn-Prediction/
│
├── churn_prediction.py
├── Churn_Modelling.csv
├── README.md
└── requirements.txt
```

---

# Random Forest Parameters

```python
RandomForestClassifier(
    n_estimators=100,
)
```

---

# Feature Scaling Formula

The project uses StandardScaler:

```math
z = (x - μ) / σ
```

Where:

* `x` = actual value
* `μ` = mean
* `σ` = standard deviation

---

# Results

The Random Forest model achieved good prediction performance on customer churn data.

The model can help businesses:

* identify risky customers
* improve retention strategies
* reduce customer loss

---

# Future Improvements

* Hyperparameter Tuning
* XGBoost Integration
* SMOTE for Class Imbalance
* Flask/Django Deployment
* Streamlit Web App

---

# Author

Hardik Prajapati

---
