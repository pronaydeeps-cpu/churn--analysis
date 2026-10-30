#  Subscription Retention & Churn Analytics

An end-to-end Data Analytics and Machine Learning project focused on understanding customer churn in a subscription-based streaming service. The project combines Exploratory Data Analysis (EDA), statistical hypothesis testing, and predictive modeling to identify the primary drivers of customer churn and recommend data-driven retention strategies.

---

##  Project Overview

Customer churn is one of the most critical business challenges faced by subscription-based platforms. Retaining existing customers is significantly more cost-effective than acquiring new ones, making churn analysis an essential component of business analytics.

This project analyzes customer demographics, subscription information, and user engagement metrics to:

- Understand customer behavior.
- Identify the factors associated with churn.
- Validate insights using statistical hypothesis testing.
- Build predictive machine learning models.
- Generate actionable business recommendations.

---

##  Objectives

- Perform comprehensive Exploratory Data Analysis (EDA).
- Identify behavioral patterns associated with customer churn.
- Validate insights using statistical tests.
- Build and compare multiple machine learning classification models.
- Evaluate model performance using standard classification metrics.
- Translate analytical findings into business recommendations.

---

##  Dataset

This project uses a **publicly available subscription customer churn dataset** sourced from Kaggle. The dataset simulates customer behavior within a subscription-based streaming service and contains **5,000 customer records**.

The dataset includes information such as:

- Customer demographics
- Subscription plans
- Watch hours
- Average watch time per day
- Last login days
- Monthly subscription fee
- Number of profiles
- Payment methods
- Device usage
- Favorite genre
- Customer churn status

---

##  Tech Stack

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn

### Development Environment

- Jupyter Notebook
- VS Code

---

# Exploratory Data Analysis

The dataset was explored to understand customer behavior and identify factors contributing to customer churn.

### Data Profiling

- Dataset inspection
- Data type verification
- Missing value analysis
- Duplicate record verification
- Descriptive statistics
- Feature distribution analysis

### Customer Distribution Analysis

- Customer churn distribution
- Age distribution
- Gender distribution
- Region distribution
- Subscription type distribution
- Device usage distribution
- Payment method distribution
- Favorite genre distribution

### Churn Analysis

Behavioral comparisons between retained and churned customers:

- Watch Hours
- Last Login Days
- Average Watch Time per Day
- Subscription Type
- Payment Method
- Region
- Device Type
- Monthly Subscription Fee
- Number of Profiles

Correlation analysis was also performed to understand relationships among numerical variables.

---

# Statistical Validation

Exploratory findings were validated using statistical hypothesis testing.

### Independent Two-Sample t-Test

Performed on numerical variables:

- Watch Hours
- Last Login Days
- Average Watch Time per Day

These tests confirmed statistically significant differences between retained and churned customers.

### Chi-Square Test of Independence

Performed on categorical variables:

- Subscription Type
- Payment Method

Both variables demonstrated statistically significant associations with customer churn.

---

#  Machine Learning

Two supervised machine learning models were developed and compared.

## Logistic Regression

Logistic Regression was selected as the baseline classification model because customer churn is a binary classification problem. The model is computationally efficient, interpretable, and provides coefficients that explain the influence of individual features on churn prediction.

### Workflow

- Feature Selection
- One-Hot Encoding
- Train-Test Split (80:20)
- Feature Scaling using StandardScaler
- Model Training
- Prediction
- Model Evaluation

### Performance

- Accuracy: **88.7%**
- ROC-AUC Score: **0.966**

---

## Random Forest Classifier

A Random Forest classifier was trained to benchmark predictive performance against Logistic Regression. Random Forest captures complex non-linear relationships by combining predictions from multiple decision trees.

### Performance

- Accuracy: **98.3%**
- ROC-AUC Score: **0.998**

Although Random Forest achieved superior predictive performance, Logistic Regression was retained as the primary analytical model because of its interpretability and ability to explain feature importance through model coefficients.

---

# Model Evaluation

The models were evaluated using multiple classification metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve
- ROC-AUC Score

---

# Key Findings

The analysis produced several important business insights:

- Higher **Average Watch Time per Day** strongly reduces customer churn.
- Higher **Watch Hours** are associated with increased customer retention.
- Longer **Last Login Days** significantly increase churn probability.
- Customers subscribed to the **Basic plan** exhibit the highest churn rate.
- Customers using **Crypto** and **Gift Card** payment methods show comparatively higher churn rates.
- Accounts with multiple profiles demonstrate better customer retention.
- Region and Device Type have minimal influence on customer churn.

Both statistical testing and machine learning models consistently identified customer engagement as the strongest predictor of subscriber retention.

---

# Business Recommendations

Based on the findings, the following recommendations are proposed:

### 1. Re-engage Inactive Customers

Develop automated email campaigns and personalized notifications for customers with prolonged inactivity.

### 2. Increase Customer Engagement

Improve personalized recommendations, curated watchlists, and content discovery to increase viewing activity.

### 3. Improve the Basic Subscription Plan

Evaluate pricing, available features, and upgrade incentives to reduce churn among Basic subscribers.

### 4. Monitor High-Risk Customer Segments

Customers using Crypto and Gift Card payment methods should be monitored for proactive retention campaigns.

### 5. Deploy Predictive Analytics

Integrate churn prediction into CRM workflows to identify high-risk customers before cancellation and enable targeted retention strategies.

---

# Project Structure

```
Subscription-Retention-Churn-Analytics
│
├── data/
│   └── netflix_customer_churn.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── reports/
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Results Summary

| Model | Accuracy | ROC-AUC |
|------|----------:|---------:|
| Logistic Regression | **88.7%** | **0.966** |
| Random Forest | **98.3%** | **0.998** |

---


# Acknowledgements

The dataset used in this project is a publicly available subscription customer churn dataset obtained from Kaggle and is intended solely for educational and analytical purposes.

---
#  Author

**Prem Sharma**


---


##  If you found this project useful or interesting, consider giving the repository a star!