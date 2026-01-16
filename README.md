# 📊 Telecom Customer Churn Prediction
**CP462 Machine Learning Project | Group 12**

> **"Did you know that acquiring a new customer costs 5 times more than retaining an existing one?"**

This project focuses on identifying patterns and predicting customer churn to help telecommunication companies maintain their customer base and optimize operational costs.

---

## 📋 Project Overview
This analysis addresses key business questions regarding customer retention and uses machine learning to predict which customers are likely to leave the service.

### ❓ Key Research Questions
1. **Which variables significantly impact a customer's decision to continue using the service?**
2. **What are the most critical factors for effective customer retention?**
3. **Are there any data quality issues, such as missing values or anomalies, that could affect the analysis?**

## 🛠️ Tech Stack
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## 🧪 Methodology
1. **Data Preprocessing:** Handled missing values and outliers to ensure data quality.
2. **Exploratory Data Analysis (EDA):** Visualized relationships between features like contract types, monthly charges, and churn status.
3. **Feature Selection:** Evaluated feature importance to improve model performance.
4. **Model Training:** Tested multiple algorithms including Naive Bayes, KNN, Logistic Regression, and Random Forest.

## 📈 Key Results & Evaluation
Since the primary goal is to minimize customer loss, we prioritized the **Recall** metric.

| Model | Features | Recall (Class 1) |
| :--- | :--- | :--- |
| **Naive Bayes** | **All Features** | **0.8356 (Best)** |
| Naive Bayes | Selected Features | 0.8194 |
| Logistic Regression | All Features | 0.5418 |
| Random Forest | All Features | 0.4960 |

**Conclusion:** The **Naive Bayes** model is the most effective for this business case because it captures the highest percentage of potential churners (83.56% Recall), allowing the company to take action before the customer leaves.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
