# Credit Risk Classification – Logistic Regression Model

##  Project Summary

This project demonstrates the use of **logistic regression** to classify loan applicants based on their credit risk. Using historical loan data from a peer-to-peer lending platform, the model predicts whether a loan is likely to be **healthy** (low risk) or **high risk** (likely to default).

The goal is to assist financial institutions in identifying risky borrowers before approving loans, minimizing default risk and increasing portfolio stability.

---
## Project Structure

- `credit_risk_classification.ipynb` – Jupyter notebook containing all data processing, model training, and evaluation
- `lending_data.csv` – Cleaned dataset of borrower financial history
- `README.md` – Summary and analysis of the project
- 
---

## Objective

> **Problem Statement:**  
Can we use borrower financial data to predict whether a loan is high-risk or healthy (low-risk)?

> **Solution:**  
Train a **logistic regression classifier** on labeled loan data and evaluate how well it performs on unseen data.

---

## 🛠️ Tools & Technologies

- **Python 3.12**
- **Pandas** – Data manipulation
- **Scikit-learn (sklearn)** – Model building, training, and evaluation
- **Jupyter Notebook** – Analysis environment

---

## 📊 Machine Learning Process

### 1. Data Preprocessing
- Loaded the dataset from `lending_data.csv`
- Split into:
  - `X`: Feature variables (loan size, income, interest rate, etc.)
  - `y`: Target label (`loan_status`: 0 = healthy, 1 = high risk)
- Used `train_test_split()` to create training (75%) and test (25%) sets

### 2. Model Development
- Applied a **Logistic Regression** model from `sklearn.linear_model`
- Trained the model using `X_train` and `y_train`
- Predicted loan status on `X_test`

### 3. Model Evaluation

### 🔹 Classification Report:

| Class | Precision | Recall | F1-score |
|-------|-----------|--------|----------|
| 0 (Healthy loans) | 1.00 | 0.99 | 1.00 |
| 1 (High-risk loans) | 0.84 | 0.94 | 0.89 |

- **Overall Accuracy**: **97%**

---

## 📈 Interpretation of Results

- **Healthy Loans (0)**: The model predicts these with near-perfect accuracy
- **High-Risk Loans (1)**: Precision of 84% and recall of 94% shows strong ability to catch risky loans
- **High F1-score** for both classes confirms the model is balanced and effective

---

## ✅ Recommendation

The logistic regression model performs with high precision and recall, especially for the business-critical task of identifying **high-risk applicants**. With an overall accuracy of 97%, this model is suitable for initial deployment in a lending environment, especially where interpretability is important.

---

##  Author

**Anqa Javed**  
Data Analytics Bootcamp, University of Toronto  
[GitHub Profile](https://github.com/AnqaJaved)

---
