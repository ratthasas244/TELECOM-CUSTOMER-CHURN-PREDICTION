# Telecom Customer Churn Prediction
**CP462 Machine Learning Project | Group 12**

"Did you know that acquiring a new customer costs 5 times more than retaining an existing one?"

## Project Overview
This project focuses on Predictive Analytics to identify customers who are likely to churn (cancel their service). In the highly competitive telecom industry, understanding the patterns of customer departure is crucial for developing targeted retention programs and minimizing revenue loss.

### Research Questions
1. Which variables significantly impact a customer's decision to continue using the service?
2. What are the most critical factors for effective customer retention?
3. Are there any data quality issues, such as missing values or anomalies, that affect the analysis?

---

## Team Members (Group 12)
1. Jirat Ukongka (ID: 66102010233)
2. Yanapat Pankasem (ID: 66102010236)
3. Benyapha Plodiueam (ID: 66102010242)
4. Rattasart Chantra (ID: 66102010244)

---

## Dataset Information
The dataset is sourced from the Telco Customer Churn dataset on Kaggle. It contains 7,043 rows and 21 features.

### Data Dictionary (Key Features):
- tenure: Number of months the customer has stayed with the company.
- Contract: The contract term (Month-to-month, One year, Two year).
- MonthlyCharges: The amount charged to the customer monthly.
- TotalCharges: The total amount charged to the customer.
- InternetService: Customer’s internet service provider (DSL, Fiber optic, No).
- TechSupport: Whether the customer has tech support (Yes, No, No internet service).
- Churn: Whether the customer churned or not (Target Variable).

---

## Tech Stack and Workflow
### Technologies:
- Language: Python
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-learn

### Workflow:
1. Data Wrangling: Checked for duplicates and missing values using missingno.
2. Exploratory Data Analysis (EDA): Analyzed customer demographics and service usage patterns.
3. Pre-processing: 
    - Handled categorical data using LabelEncoder and OneHotEncoder.
    - Scaled numerical features using MinMaxScaler and StandardScaler.
4. Model Training: Implemented 4 algorithms:
    - Naive Bayes (GaussianNB)
    - K-Nearest Neighbors (KNN)
    - Logistic Regression
    - Random Forest Classifier

---

## Model Performance and Evaluation
We prioritized the Recall metric for the positive class (Churn = Yes) because the cost of missing a customer who is about to leave is higher than incorrectly identifying a loyal customer as a churner.

| Model | Features | Recall (Churn = Yes) |
| :--- | :--- | :--- |
| **Naive Bayes** | **All Features** | **0.8356 (Highest)** |
| Naive Bayes | Selected Features | 0.8194 |
| Logistic Regression | All Features | 0.5418 |
| KNN | All Features | 0.5121 |
| Random Forest | All Features | 0.4960 |

### Key Insights:
- Best Model: Naive Bayes provided the highest Recall (83.56%), making it the most suitable model for proactive retention strategies.
- Contract Type: Customers with "Month-to-month" contracts have a significantly higher churn rate compared to those with long-term contracts.
- Service Factors: Lack of TechSupport and OnlineSecurity services are strong indicators of potential churn.

---

## How to Use
1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed: `pip install pandas numpy seaborn matplotlib scikit-learn plotly`.
3. Open `CP462_Project_Group12_Final.ipynb` in Google Colab or Jupyter Notebook.
4. Run the cells to reproduce the analysis and model evaluation.

---
*This project is part of the CP462 course requirement.*
