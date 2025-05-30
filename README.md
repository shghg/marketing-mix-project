# 📊 Marketing Mix Analysis with Python

[![Built with Python](https://img.shields.io/badge/Built%20with-Python-blue)](https://www.python.org/)
[![Project Type](https://img.shields.io/badge/Type-Bootcamp%20Project-purple)]()
[![Status: Completed](https://img.shields.io/badge/Status-Completed-brightgreen)]()

---

## 🧠 Overview

This project was developed as part of my **AI & Machine Learning Bootcamp**, where I conducted a comprehensive analysis of a **marketing campaign dataset** to extract **data-driven business insights**.

The goal was to evaluate customer behavior and marketing effectiveness using the **4 Ps of Marketing** — **Product, Price, Place, Promotion** — plus **People**, to guide strategy decisions.

---

## 🎯 Objectives

- 🔹 Clean, transform, and engineer features from raw marketing data  
- 🔹 Visualize distributions and detect outliers  
- 🔹 Encode categorical variables effectively  
- 🔹 Perform hypothesis testing to support or reject marketing assumptions  
- 🔹 Deliver actionable insights using Python visualizations and statistics  

---

## 📁 Dataset Overview

The dataset contains information on **over 2,000 customers**, including demographics, spending behavior, campaign responses, and channel preferences.

### Key Fields:
- **Demographics**: `Income`, `Education`, `Marital_Status`, `Year_Birth`
- **Product Spending**: `MntWines`, `MntFruits`, ..., `MntGoldProds`
- **Purchases**: `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases`
- **Campaign Response**: `Response` (whether the last campaign was accepted)

---

## 🛠️ Key Tasks Performed

### ✅ 1. Data Cleaning
- Removed formatting from `Income` (e.g., "$84,000" → 84000.0)
- Parsed `Dt_Customer` to datetime
- Imputed missing `Income` values using group means by `Education` and `Marital_Status`

### ✅ 2. Feature Engineering
- Created new features:
  - `Total_Children = Kidhome + Teenhome`
  - `Age = Current Year - Year_Birth`
  - `Total_Spending = Sum of product expenditures`
  - `Total_Purchases = Sum of all purchase channels`

### ✅ 3. Outlier Detection & Treatment
- Applied **IQR (Interquartile Range) method** for capping outliers:
  ```
  IQR = Q3 - Q1
  Lower Bound = Q1 - 1.5 * IQR
  Upper Bound = Q3 + 1.5 * IQR
  ```

### ✅ 4. Categorical Encoding
- Used **ordinal encoding** for `Education`  
- Applied **one-hot encoding** for `Marital_Status` and `Country`

### ✅ 5. Hypothesis Testing
- 📌 Do older customers shop more in-store?
- 📌 Do customers with children prefer online purchases?
- 📌 Is there cannibalization between store and online shopping?
- 📌 Do US-based customers spend more on average?

### ✅ 6. Visualizations & Insights
- Heatmap of feature correlations
- Product category revenue rankings
- Campaign response rates by age, location, and children
- Complaint distribution by education level

---

## 🔍 Insights & Takeaways

- Real-world experience with **feature engineering** and **outlier treatment**
- Applied **hypothesis testing** using statistical methods (t-tests, Pearson correlation)
- Learned practical techniques for **missing data imputation**
- Reinforced the value of **data visualization for business storytelling**

---

## 🧰 Tools Used

- **Python 3.x**
- **Pandas, NumPy** – data handling & transformation  
- **Matplotlib, Seaborn** – visualization  
- **SciPy, Statsmodels** – statistical testing  
- **Jupyter Notebook** – development environment

---

## 📌 What You Can Learn from This

Whether you're a data scientist, marketing analyst, or student, this project offers insights into:
- How to structure a real-world marketing dataset
- Feature extraction and domain-specific analysis
- Turning business questions into testable hypotheses
- Making data-driven marketing decisions
