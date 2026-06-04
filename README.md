# 📉 Customer Churn Prediction

> Predicting which customers are likely to leave — before they do.

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?style=flat-square&logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat-square&logo=pandas)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

---

## 📌 Overview

Customer churn is one of the most critical challenges in subscription-based businesses. This project uses **Exploratory Data Analysis (EDA)** and **Machine Learning** to identify patterns in customer behavior and predict which customers are at risk of leaving a telecom company.

The dataset contains **7,043 customer records** with demographic, service, and billing information.

---

## 🎯 Objectives

- Understand the key factors that drive customer churn
- Clean and preprocess real-world telecom data
- Visualize patterns across contract types, services, and billing methods
- Build a Logistic Regression model to predict churn
- Derive actionable business recommendations from the findings

---

## 📂 Project Structure

```
customer-churn-prediction/
│
├── customer_Churn_Prediction.ipynb   # Main Jupyter Notebook
├── customer_churn.csv                # Dataset
└── README.md                         # Project documentation
```

---

## 📊 Dataset

| Feature | Description |
|---|---|
| `customerID` | Unique customer identifier |
| `tenure` | Number of months with the company |
| `Contract` | Contract type (Month-to-month, One year, Two year) |
| `MonthlyCharges` | Monthly billing amount |
| `TotalCharges` | Total amount billed |
| `InternetService` | Type of internet service |
| `PaymentMethod` | Payment method used |
| `Churn` | Target variable — Yes/No |

**Source:** Telco Customer Churn Dataset

---

## 🔍 Key Findings from EDA

| Factor | Finding |
|---|---|
| 📋 Contract Type | Month-to-month customers churn the most |
| 🌐 Internet Service | Fiber optic users show the highest churn |
| 💳 Payment Method | Electronic check users are most likely to churn |
| 💰 Monthly Charges | Higher charges correlate with higher churn |
| ⏱️ Tenure | New customers are significantly more likely to leave |

---

## 🤖 Machine Learning Model

**Algorithm:** Logistic Regression

| Metric | Score |
|---|---|
| Accuracy | 78.82% |
| F1-Score (Retained) | 0.86 |
| F1-Score (Churned) | 0.57 |

The model correctly identifies retained customers with high confidence. Performance on churned customers highlights the impact of class imbalance (~26.5% churn rate) — a direction for future improvement.

---

## 🛠️ Tech Stack

- **Python** — Core language
- **Pandas & NumPy** — Data manipulation
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/customer-churn-prediction.git
   cd customer-churn-prediction
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. **Open the notebook**
   ```bash
   jupyter notebook customer_Churn_Prediction.ipynb
   ```

---

## 💡 Business Recommendations

- **Promote long-term contracts** through discounts and loyalty rewards to reduce month-to-month churn
- **Investigate fiber optic service quality** — pricing or performance issues may be driving dissatisfaction
- **Incentivize automatic payments** — customers on auto-pay show significantly better retention
- **Focus on early onboarding** — new customers are the most vulnerable; personalized support in the first 3–6 months can make a big difference
- **Re-evaluate pricing** for high monthly charge customers who may feel the service isn't worth the cost

---

## 🔮 Future Improvements

- [ ] Handle class imbalance using SMOTE or `class_weight='balanced'`
- [ ] Add feature scaling with StandardScaler
- [ ] Test Random Forest and XGBoost models
- [ ] Evaluate with ROC-AUC instead of accuracy alone
- [ ] Add K-Fold Cross-Validation for more reliable performance estimates

---

## 👤 Author

**Shibina Sharin**
- GitHub: github.com/shibinasharin
- LinkedIn: linkedin.com/in/shibina-sharin-7a7705375

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
