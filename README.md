# 💼 Credit Risk Classification – Module 20 Challenge

By: **Anqa Javed**

---

## 📌 Overview

The goal of this project was to build a machine learning model that can accurately classify loan applications as either **low risk** or **high risk**.  
The dataset comes from a peer-to-peer lending platform and includes financial data such as loan size, interest rate, borrower income, and debt level.  
We used a **Logistic Regression model** to predict whether a borrower is likely to default on a loan.

---

## 📊 Machine Learning Process

### ✔️ Data Preparation
- Loaded the dataset from `lending_data.csv`
- Separated the data into:
  - `X` (features): borrower financial data
  - `y` (labels): loan_status (0 = healthy, 1 = high-risk)
- Split the data into **training (75%)** and **testing (25%)** sets using `train_test_split`

### ✔️ Model Training
- Trained a **LogisticRegression** model using the training data (`X_train`, `y_train`)

### ✔️ Predictions & Evaluation
- Predicted loan risk using the test set (`X_test`)
- Evaluated the model using a **confusion matrix** and **classification report**

---

## 📈 Results

### 🔹 Classification Report:

| Class | Precision | Recall | F1-score |
|-------|-----------|--------|----------|
| 0 (Healthy loans) | 1.00 | 0.99 | 1.00 |
| 1 (High-risk loans) | 0.84 | 0.94 | 0.89 |

- **Overall Accuracy**: **97%**

---

## 🧠 Summary and Recommendation

The model performs extremely well on both healthy and high-risk loans.  
It correctly identifies 99% of all healthy loans and 94% of all high-risk ones, with high precision for both.  
Because of the strong balance between **accuracy, precision, and recall**, I recommend this model for use in real-world loan approval scenarios.  
It will help the company reduce default risk while still approving creditworthy borrowers.

---

## 🗂️ Project Files

- `Credit_Risk/credit_risk_classification.ipynb` – Jupyter notebook containing the full ML workflow
- `Credit_Risk/lending_data.csv` – Dataset used for training and testing
- `Credit_Risk/README.md` – This file, with a full analysis report

---

## ✅ Tools Used

- Python  
- Pandas  
- Scikit-learn (LogisticRegression, train_test_split, confusion_matrix, classification_report)  
- Jupyter Notebook

---

## 📬 Contact

This project was submitted as part of the University of Toronto Data Analytics Bootcamp.  
Created and maintained by [Anqa Javed](https://github.com/AnqaJaved)
