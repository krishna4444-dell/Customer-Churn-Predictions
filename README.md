# 📊 Customer Churn Prediction

## 📌 Project Overview

Customer churn is one of the biggest challenges faced by subscription-based businesses. Losing existing customers directly impacts company revenue and increases customer acquisition costs.

The objective of this project is to predict whether a customer is likely to churn using customer demographics, subscription details, billing information, and service usage. By identifying customers at risk of leaving, the company can proactively take retention actions such as discounts, loyalty programs, and personalized offers.

---

## 🎯 Business Problem

A telecom company wants to identify customers who are likely to cancel their subscription.

Instead of waiting until customers leave, the company can use machine learning to predict high-risk customers and improve customer retention through targeted marketing strategies.

---

## 📂 Dataset

* **Dataset:** Telecom Customer Churn Dataset
* **Source:** Kaggle
* **Rows:** 7,043
* **Columns:** 33

The dataset contains information about:

* Customer demographics
* Subscription details
* Billing information
* Internet services
* Payment methods
* Contract types
* Customer churn status

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Joblib

---

## 📈 Project Workflow

### 1. Data Understanding

* Loaded the dataset
* Studied every feature
* Checked data types
* Identified missing values
* Analyzed target distribution

### 2. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand customer behavior.

Key observations included:

* Customers with shorter tenure churn more frequently.
* Month-to-month contracts have the highest churn rate.
* Customers with higher monthly charges are more likely to churn.
* Customers without technical support show higher churn.
* Fiber optic users have a higher churn rate compared to other internet service types.

---

### 3. Data Preprocessing

* Removed unnecessary features
* Removed data leakage features
* Converted categorical features using One-Hot Encoding
* Applied feature scaling where appropriate
* Built a preprocessing pipeline
* Split data into training and testing sets

---

### 4. Machine Learning Models

The following models were trained and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

Hyperparameter tuning was performed using **GridSearchCV** with cross-validation.

---

## 📊 Model Evaluation

Evaluation metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

Since customer churn prediction focuses on identifying customers before they leave, **Recall** was considered the primary evaluation metric.

### Best XGBoost Performance

* **Training Accuracy:** 83.55%
* **Testing Accuracy:** 79.91%
* **ROC-AUC Score:** 0.854

---

## 🔍 Feature Importance

The most influential features identified by XGBoost include:

* Contract Type (Month-to-Month)
* Internet Service (Fiber Optic)
* Technical Support
* Online Security
* Tenure
* Monthly Charges
* Total Charges
* Payment Method

---

## 💡 Business Insights

The analysis suggests that customers are more likely to churn when they:

* Have a month-to-month contract
* Are new customers with shorter tenure
* Pay higher monthly charges
* Do not have technical support
* Use fiber optic internet service
* Pay using electronic checks

### Recommendations

To reduce customer churn, the company should:

* Encourage long-term contracts through discounts.
* Provide proactive technical support.
* Offer loyalty rewards to new customers.
* Create personalized retention campaigns for high-risk customers.
* Improve customer experience for fiber optic users.

---

## 🚀 Future Improvements

* Deploy the model using Flask or FastAPI.
* Build an interactive prediction web application.
* Explain predictions using SHAP values.
* Automate model retraining with updated customer data.

---

## 📁 Repository Structure

```
Customer-Churn-Prediction/
│
├── data/
├── notebooks/
├── models/
├── images/
├── README.md
├── requirements.txt
├── .gitignore
└── app.py
```

---

## 👨‍💻 Author

**krishna kishore**

Aspiring Data Scientist passionate about Machine Learning, Data Analysis, and solving real-world business problems using AI.
