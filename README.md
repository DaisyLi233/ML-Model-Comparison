# 🏎️ Predicting Used Car Prices with Machine Learning

Pricing used vehicles accurately is a challenging problem due to complex market dynamics, heterogeneous car attributes, and highly skewed price distributions.  
This project uses a publicly available dataset from the Indian used-car market to investigate how different machine learning models perform on predicting used vehicle prices.

---

## 🔍 Project Overview

We perform a complete end-to-end machine learning workflow, including:

- **Exploratory Data Analysis (EDA)**  
- **Feature Engineering** (e.g., creating a brand feature)  
- **Duplicate removal**  
- **Brand-specific outlier handling**  
- **Log transformation** on the target variable to reduce skewness  

The goal is to benchmark model performance across multiple algorithms and understand how different models behave on a long-tailed price distribution.

---

## 🤖 Models Compared

We evaluate five supervised regression models:

- **Linear Regression / Polynomial Regression**  
- **Support Vector Regression (SVR)**  
- **Random Forest Regressor**  
- **AdaBoost Regressor**  
- **Gradient Boosting Regressor**

Models are compared using:

- **R²**
- **RMSE** (on both log-transformed and original price scales)

---

## 📈 Key Findings

- **Gradient Boosting** and **AdaBoost** achieve the best overall predictive performance.  
- A simple **Linear Regression with Ridge regularization** provides a surprisingly strong and stable baseline.  
- **Random Forest** struggles with **rare, high-priced vehicles**, leading to underperformance on the long tail of the distribution.  
- Traditional metrics (e.g., R²) can be **misleading on heavily skewed data**, emphasizing the importance of combining:
  - numerical score comparison  
  - **residual-based visual diagnostics**

---

## 📄 Full Article

For more details, in-depth analysis, and visual explanations, see the full article:  
👉 https://www.linkedin.com/pulse/predicting-used-car-prices-machine-learning-insights-from-siyi-li-cj8ze/?trackingId=C%2F7h7PukTMW58JvWareXUw%3D%3D

