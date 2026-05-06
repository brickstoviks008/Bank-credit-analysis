# 💳 Credit Risk Modeling Project


![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-yellow)
![XGBoost](https://img.shields.io/badge/XGBoost-Gradient%20Boosting-green)


---

## 🚀 Project Overview

This project focuses on building a **machine learning model** to predict the probability of customer default using financial and behavioral data.

The goal is to help financial institutions:
- Identify **high-risk customers**
- Improve **credit decision-making**
- Reduce **default risk**

---

## 🎯 Objective

To develop a predictive model that classifies customers into:
- ✅ **Good Customers (0)**
- ❌ **Bad Customers (1)**

Based on their historical financial and transactional behavior.

---

## 📂 Dataset Description

The dataset consists of:

### 🧾 Customer Demographics
- Anonymized features (`feature_1` to `feature_79`)

### 💰 Customer Account Data
- Balance details
- Credit limits
- Payment behavior
- Past dues

---

## ⚠️ Key Data Challenges

- 🔴 Severe class imbalance (~96% good, ~4% bad)
- 🔧 Numeric columns stored as object type
- 📅 Date parsing inconsistencies
- ♾️ Infinite values from feature engineering
- ❓ Missing values across multiple features

---

## 🧹 Data Preprocessing

✔ Converted data types (`object → numeric`)  
✔ Parsed date columns and extracted useful features  
✔ Handled missing values using imputation  
✔ Replaced infinite values (`inf`, `-inf`)  
✔ Encoded categorical variables  

---

## ⚙️ Feature Engineering

Key features created:

- 📊 Aggregated customer-level metrics (sum, mean)
- 📅 Payment behavior features
- 💳 Balance & credit utilization indicators
- ⏱️ Time-based features (payment gaps)

---

## 🤖 Model Development

### Model Used:
👉 **XGBoost Classifier**

### Why XGBoost?
- Handles non-linear relationships
- Works well with tabular data
- Robust to noisy features

---

## ⚖️ Handling Class Imbalance

Used:
- `scale_pos_weight` to balance minority class impact

---

## 📈 Model Evaluation

### Metrics Used:
- 🎯 **AUC (Area Under Curve)**
- 📉 **Gini Coefficient**
Gini = 2 × AUC - 1


---

## 📊 Decile Analysis

Customers were ranked based on predicted risk and divided into 10 groups.

### 🔍 Observations:

- Partial separation of high-risk customers
- Lack of strong monotonic trend across deciles
- Indicates moderate predictive power

---

## 🧠 Key Insights

- 📌 Data quality significantly impacts model performance  
- 📌 Feature engineering plays a crucial role  
- 📌 Class imbalance requires careful handling  
- 📌 Model captures some signal but lacks strong separation  

---

## 📉 Limitations

- ⚠️ Weak decile monotonicity
- ⚠️ Moderate model performance
- ⚠️ High feature noise due to anonymized variables

---

## 🔮 Future Improvements

- 🚀 Hyperparameter tuning  
- 🧪 Advanced feature engineering  
- 🔄 Try alternative models (LightGBM, CatBoost)  
- ⚖️ Use SMOTE or advanced imbalance techniques  
- 🎯 Feature selection to remove noise  

---

## 🏁 Conclusion

This project successfully demonstrates:

✔ End-to-end machine learning pipeline  
✔ Real-world data cleaning challenges  
✔ Model building and evaluation  

However:

👉 The model shows **moderate predictive capability** and requires further optimization for production use.

---

## 📌 Tech Stack

- 🐍 Python  
- 📊 Pandas, NumPy  
- 🤖 Scikit-learn  
- ⚡ XGBoost  

---

## 🙌 Final Note

This project highlights the importance of:
- Data preprocessing 🧹  
- Feature engineering ⚙️  
- Model evaluation 📊  

in building a reliable credit risk model.

---

## ⭐ AUTHOR
  ## VIKASINI D
