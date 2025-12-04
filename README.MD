# Customer Churn Analysis & Prediction

This project analyzes telecom customer churn and builds a predictive machine learning model to identify customers likely to leave the service. The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and hyperparameter tuning.
"C:\Users\sawma\Pictures\Screenshots\Screenshot 2025-12-04 085220.png"

---

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Dataset Description](#dataset-description)  
3. [Data Cleaning & Preprocessing](#data-cleaning--preprocessing)  
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
5. [Feature Engineering](#feature-engineering)  
6. [Model Development](#model-development)  
7. [Model Improvement](#model-improvement)  
8. [Hyperparameter Tuning](#hyperparameter-tuning)  
9. [Feature Importance](#feature-importance)  
10. [Model Deployment](#model-deployment)  
11. [How to Run](#how-to-run)
12. [Contact](#contact)

---

## Project Overview
Customer churn prediction helps telecom companies understand why customers leave and enables strategies to retain them. This project uses statistical analysis and machine learning to build a robust churn prediction system.

---

## Dataset Description
The dataset contains customer-level information such as telecom services used, contract details, payment methods, tenure, and churn status.

Key target variable:  
**Churn** – whether the customer exited the service.

---

## Data Cleaning & Preprocessing

Key operations performed:

- Replaced blank values in *TotalCharges* with `0` when tenure was `0`.
- Converted the `SeniorCitizen` column from `0/1` to `Yes/No` for better readability.
- Categorical variables encoded.
- Missing values handled.
- Train-test split applied for modeling.

---

## Exploratory Data Analysis (EDA)

Insights extracted from visual exploration:

- Around **26.54%** of customers have churned.
- Senior citizens show a higher churn tendency.
- Customers with short tenure (1–2 months) churn more often.
- Month-to-month contracts show significantly higher churn compared to 1–2 year plans.
- Customers who rely only on core phone/internet services churn more.
- Electronic check payment method has the highest churn rate.

---

## Feature Engineering

- Target variable encoded.
- Categorical features transformed using suitable encoders.
- Numerical features scaled where necessary.

---

## Model Development

Models evaluated:

- **Logistic Regression**
- **Random Forest Classifier**

Both models were trained and compared on accuracy, precision, recall, and F1-score.

---

## Model Improvement

SMOTE (Synthetic Minority Oversampling Technique) was applied to address the churn class imbalance:

- Slight decrease in overall accuracy.
- Significant improvement in **recall**, allowing better identification of churners (business-critical objective).

---

## Hyperparameter Tuning

GridSearchCV was applied on the Random Forest model to find optimal hyperparameters:

- Tuned model produced higher recall.
- Improved generalization.
- Better churn detection performance.

---

## Feature Importance

Key drivers of churn (based on the best-performing Random Forest model):

- Tenure
- Monthly charges
- Contract type
- Internet service
- Payment method

Feature importance visualization was plotted to interpret model decisions.

---

## Model Deployment

Steps included:

- Saving the final trained model.
- Preparing it for real-world prediction use.
- Exporting artifacts for deployment (e.g., Pickle file).

---

## How to Run

working yet.....

## Contact

📧 Email : sawmar044@gmail.com

🔗 Linkedin : https://www.linkedin.com/in/balram-shah/
