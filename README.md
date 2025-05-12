# Credit Risk Classification – Logistic Regression Model

This project demonstrates how logistic regression can be applied to predict the credit risk of borrowers based on their financial attributes. The goal is to help lending institutions classify applicants as low or high risk before issuing a loan.

## Overview

Using data from a peer-to-peer lending platform, this project trains and evaluates a supervised machine learning model to predict whether a loan is likely to default.

The logistic regression model was chosen for its efficiency and interpretability when working with binary classification tasks.

## Project Structure

- `credit_risk_classification.ipynb` – Jupyter notebook containing all data processing, model training, and evaluation
- `lending_data.csv` – Cleaned dataset of borrower financial history
- `README.md` – Summary and analysis of the project

## Tools & Libraries

- Python  
- Pandas  
- Scikit-learn  
- Jupyter Notebook  

## Process

1. Loaded and inspected the dataset
2. Prepared features (`X`) and labels (`y`) for modeling
3. Split data into training and testing sets
4. Trained a logistic regression model using `LogisticRegression`
5. Evaluated model performance using a confusion matrix and classification report

## Results

**Classification Report Highlights:**

- Accuracy: **97%**
- Precision (high-risk loans): **0.84**
- Recall (high-risk loans): **0.94**
- Precision (healthy loans): **1.00**
- Recall (healthy loans): **0.99**

These results indicate a high-performing model with excellent ability to distinguish between low and high credit risk applicants.

## Conclusion

The logistic regression model demonstrates strong performance for credit risk classification. Its accuracy and recall make it a good candidate for deployment in a real-world lending environment.

## Author

**Anqa Javed**  
[GitHub Portfolio](https://github.com/AnqaJaved)
