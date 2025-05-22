# Credit Risk Classification – Logistic Regression Model

## 📌 Project Summary

This project applies a logistic regression model to classify loan applicants as either **high-risk** or **low-risk** based on financial attributes. Using historical data from a peer-to-peer lending platform, the model helps predict the likelihood of default before a loan is issued.

This approach supports lending institutions in making smarter, data-driven decisions and reducing default-related losses.

---

## 🧾 Project Structure

- `credit_risk_classification.ipynb` – Jupyter notebook with full code, data processing, training, and model evaluation  
- `lending_data.csv` – Clean dataset of borrower loan and financial attributes  
- `README.md` – Project summary, methodology, and evaluation report

---

## 🎯 Objective

**Problem Statement:**  
Can we accurately predict whether a loan will default using a borrower’s financial profile?

**Solution:**  
We use logistic regression to build a binary classifier based on borrower data. The model is trained, validated, and evaluated using standard classification metrics to assess real-world performance.

---

## 🔧 Tools & Technologies Used

- Python 3.12  
- Pandas – for data preprocessing  
- scikit-learn – for model building and evaluation  
- Jupyter Notebook – for analysis and documentation

---

## ⚙️ Machine Learning Process

### 1. Data Preparation

- Loaded data from `lending_data.csv`
- Target variable: `loan_status`  
  - 0 = Healthy loan  
  - 1 = High-risk loan  
- Features include:  
  `loan_size`, `interest_rate`, `borrower_income`, `debt_to_income`, `num_of_accounts`, `derogatory_marks`, `total_debt`
- Data was split:  
  - 75% training set  
  - 25% testing set

---

### 2. Model Development

- Model: `LogisticRegression()` from scikit-learn  
- Trained using `X_train`, `y_train`  
- Predictions made on `X_test`  
- Hyperparameters:  
  - `random_state=1`  
  - `max_iter=1000` to avoid convergence issues

---

### 3. Model Evaluation

#### Classification Report:

| Class              | Precision | Recall | F1-score |
|--------------------|-----------|--------|----------|
| 0 (Healthy loans)  | 1.00      | 0.99   | 1.00     |
| 1 (High-risk loans)| 0.84      | 0.94   | 0.89     |

- **Overall Accuracy:** 97%

#### Confusion Matrix:

The model demonstrates strong recall and precision for both classes, especially high-risk loans (class 1), which are critical in risk management.

---

## ✅ Final Recommendation

The logistic regression model is performing with **excellent accuracy and strong F1-scores**, especially for high-risk loans. Given its:

- **High interpretability**
- **Strong recall for risky loans**
- **Clean and reproducible structure**

...this model is well-suited for initial deployment in a financial screening environment or as a baseline model in larger risk prediction pipelines.

---

## 📇 Author

**Anqa Javed**  
University of Toronto – Data Analytics Bootcamp  
[GitHub Profile](https://github.com/AnqaJaved)
