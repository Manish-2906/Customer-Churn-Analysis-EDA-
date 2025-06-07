# 📊 Customer Churn Analysis – Exploratory Data Analysis (EDA)

This project involves a detailed **Exploratory Data Analysis (EDA)** on a telecom customer dataset to identify key factors contributing to customer churn and help businesses take action to improve retention.

---

## 📝 Dataset Overview

- **Dataset Size**: 7,043 rows × 23 columns  
- **Target Variable**: `Churn` (Yes / No)
- **Goal**: Understand customer behavior and churn drivers through visualization and statistics.

---

## 🔧 Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **SciPy**

---

## 🧹 Data Preprocessing

- Removed whitespace from column headers.
- Replaced blank entries in `TotalCharges` with 0 and converted to `float`.
- Converted `SeniorCitizen` values from `0/1` to `No/Yes`.
- Verified:
  - No missing values
  - No duplicate rows
  - `customerID` is unique

---

## 📊 Descriptive Statistics

| Feature          | Skew | Kurtosis | Key Insight |
|------------------|------|----------|-------------|
| `tenure`         | ➕ (Right) | -1.38     | Most churn happens within the first year |
| `MonthlyCharges` | ➖ (Left)  | -1.26     | Moderate to high monthly charges dominate |
| `TotalCharges`   | ➕ (Right) | -0.23     | High-value customers have higher total charges |

📌 All distributions are **platykurtic** → Flatter and more spread out than normal.

---

## 📉 Churn Distribution

- **26.5% of customers have churned**
- Class imbalance present but manageable.

---

## 📊 Key Visual Insights

### 1. 📅 Tenure vs Churn
- Customers with **<12 months tenure** show the highest churn.
  
### 2. 👵 Senior Citizens
- Higher churn among **senior customers**.

### 3. 📑 Contract Type
- **Month-to-month contracts** have significantly higher churn than long-term contracts.

### 4. 💳 Payment Method
- **Electronic check** users are more likely to churn.

### 5. 🌐 Services Impact
- Customers **not using services** like OnlineSecurity, TechSupport, StreamingTV show higher churn.

---

## 🔍 Summary of Business Insights

- 📉 Focus on retaining customers in their **first year**.
- 👴 Target **senior citizens** with loyalty plans.
- 🤝 Promote **yearly contracts** and **auto-pay methods**.
- 🔐 Upsell **security and support services** to reduce churn.



