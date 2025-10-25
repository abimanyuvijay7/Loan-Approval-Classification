# 🏦 Loan Approval Classification

This project predicts whether a loan application will be approved or rejected using demographic, financial, and credit-related attributes.  
It was completed as part of the **BUDT 704: Data Processing and Analysis in Python** course at the **University of Maryland**.

---

## Project Overview

Loan defaults and approvals have major implications for financial institutions.  
This project builds multiple machine learning models to predict loan approval status based on applicant characteristics such as income, credit history, and loan-to-income ratio.

**Objectives:**
- Identify key drivers behind loan approvals.  
- Compare different machine learning models (Logistic Regression, Decision Tree, Random Forest).  
- Recommend insights for better credit risk management.

---

## Dataset Description
The dataset consists of **45,000 records** and **14 variables**, including:

| Feature | Description |
|----------|--------------|
| person_age | Age of the applicant |
| person_gender | Gender of the applicant |
| person_education | Education level |
| person_income | Annual income |
| person_emp_exp | Employment experience (years) |
| person_home_ownership | Home ownership status |
| loan_amnt | Loan amount requested |
| loan_int_rate | Interest rate applied |
| loan_percent_income | Loan amount as % of annual income |
| cb_person_cred_hist_length | Length of credit history (years) |
| credit_score | Applicant’s credit score |
| previous_loan_defaults_on_file | Previous loan default status (Yes/No) |
| loan_status | Target variable (1 = Approved, 0 = Rejected) |

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Removed anomalies and capped outliers  
- Encoded categorical variables (e.g., gender, default status)  
- Created derived features like `age_category`  
- Validated data integrity  

### 2. Exploratory Data Analysis
- Distribution analysis (age, education, home ownership, loan intent)  
- Correlation heatmaps and univariate histograms  
- Identified trends between income, credit score, and loan approval  

### 3. Modeling
Trained and compared four models:
- Linear Regression  
- Logistic Regression  
- Decision Tree  
- Random Forest  

### 4. Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Results

| Model | Accuracy | Key Notes |
|--------|-----------|------------|
| Logistic Regression | 0.83 | Struggled with Class 1 (loan approvals) |
| Decision Tree | 0.90 | Balanced and interpretable |
| Random Forest | **0.93** | Best performer overall |

**Key Predictors of Loan Approval:**
- Credit score  
- Loan-to-income ratio  
- Credit history length  

---

## Business Insights
- Smaller loans (< $10,000) have higher approval rates.  
- Applicants aged 25–32 with moderate incomes (~$80,000) dominate approvals.  
- Credit scores above 600 correlate strongly with approval.  
- Random Forest provides the most reliable automated decision model.  

---
