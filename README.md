# 💳 Credit Score Classification & Analysis

## 📌 Project Overview

This project focuses on **analyzing credit score data** and building a **machine learning model to classify credit scores** based on customer financial information. It includes **Exploratory Data Analysis (EDA), correlation analysis, and predictive modeling**.

The dataset contains **100,000 records** with **28 features** including demographic, financial, and credit-related information.

---

## 🎯 Objectives

* Analyze patterns in credit score distribution
* Explore relationships between financial metrics and credit scores
* Visualize data using interactive and static plots
* Build a **Random Forest classifier** to predict credit scores
* Provide a **user-friendly credit score prediction interface**

---

## 🗂 Dataset

* **Source:** `Credit Score Data.csv`

* **Records:** 100,000

* **Features:** 28 columns including:

  * Personal Info: `ID`, `Customer_ID`, `Name`, `Age`, `SSN`, `Occupation`
  * Financial Info: `Annual_Income`, `Monthly_Inhand_Salary`, `Num_Bank_Accounts`, `Num_Credit_Card`, `Outstanding_Debt`, `Monthly_Balance`
  * Credit Info: `Credit_Mix`, `Payment_of_Min_Amount`, `Delay_from_due_date`, `Num_of_Delayed_Payment`, `Credit_Score`

* **Target Variable:** `Credit_Score` (`Poor`, `Standard`, `Good`)

---

## 🛠 Tech Stack & Libraries

* **Python**
* **Pandas, NumPy** – Data handling & processing
* **Matplotlib, Seaborn** – Visualization
* **Plotly** – Interactive visualizations
* **Scikit-learn** – Random Forest classifier, train-test split

---

## 📊 Exploratory Data Analysis (EDA)

### ✔ Credit Score Distribution

* Count plots for credit scores
* Credit score frequency by **Occupation, Payment Behaviour**

### ✔ Financial Feature Analysis

* Boxplots showing relationships between **Credit Score** and:

  * Annual Income
  * Monthly In-hand Salary
  * Number of Bank Accounts
  * Number of Credit Cards
  * Interest Rate
  * Number of Loans
  * Delay from Due Date
  * Outstanding Debt
  * Credit Utilization Ratio
  * Credit History Age
  * Monthly Balance

### ✔ Correlation Analysis

* Heatmap of correlations between numerical features
* Key insights for predictive modeling

---

## 🤖 Machine Learning Model

### 🔧 Methodology

* **Target:** `Credit_Score`

* **Features Used:**

  `Annual_Income, Monthly_Inhand_Salary, Num_Bank_Accounts, Num_Credit_Card, Interest_Rate, Num_of_Loan, Delay_from_due_date, Num_of_Delayed_Payment, Credit_Mix, Outstanding_Debt, Credit_History_Age, Monthly_Balance`

* **Model:** `RandomForestClassifier`

* **Train-Test Split:** 67%-33%

* **Evaluation:** Predicts `Poor`, `Standard`, or `Good` credit score

### 📌 Example Prediction

```python
# Input sample features
features = np.array([[19114.12, 2410.0, 2, 1, 10.5, 1, 0, 0, 1, 5000, 5, 1500]])
predicted_score = model.predict(features)
print("Predicted Credit Score = ", predicted_score)
```

*Output:*
`Predicted Credit Score = ['Good']`

---

## 📈 Visualizations

* Interactive **Plotly boxplots** for credit score vs financial features
* Scatter plots for **Annual Income vs Monthly Balance**
* Correlation heatmap for numerical variables
* Count plots for **Payment Behaviour vs Credit Score**

---

## 📂 Project Structure

```
Credit_Score_Classification/
│
├── Credit Score Data.csv
├── Credit_Score_Analysis_and_Classification.pdf
├── requirements(CC).txt
├── README.md
```

---

## 📌 Future Improvements

* Encode categorical features using **One-Hot Encoding or Label Encoding**
* Explore **other classification algorithms** (XGBoost, Gradient Boosting)
* Deploy as **web application using Streamlit or Flask**
* Incorporate **feature scaling** for improved model accuracy

---

## ⭐ Acknowledgements

* Dataset Source: Credit Score Data
* Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn, Plotly

---
