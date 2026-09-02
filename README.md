# eda_ibm_telco_churn_analysis_python

# Customer Churn Exploratory Data Analysis
An exploratory data analysis project investigating the key customer demographics, services, contracts, tenure, and billing factors associated with customer churn in a telecommunications company.

## Project Overview
Customer churn is a major business challenge for subscription-based companies. Losing existing customers can directly affect revenue and increase the cost of acquiring new customers.
This project performs Exploratory Data Analysis (EDA) on the IBM Telco Customer Churn dataset to identify patterns and factors associated with customer churn. The analysis focuses on understanding which customer groups are more likely to churn and what characteristics are associated with higher churn rates.
Note: This project identifies associations and patterns in the data and does not claim that the observed variables directly cause customer churn.
# Business Question
What factors and customer characteristics are associated with a higher likelihood of customer churn?

## Dataset
The dataset contains customer-level information from a telecommunications company, including:
- Customer demographics
- Account and relationship information
- Internet and phone services
- Contract type
- Billing and payment behavior
- Monthly and total charges
- Customer churn status

# Key Variables Analysed
## Category                        Variables          
Customer Demographics            Gender, SeniorCitizen, Partner, Dependents
Customer Account                 Tenure, Contract
Services                         InternetService, OnlineSecurity, TechSupport
Billing                          MonthlyCharges, PaperlessBilling, PaymentMethod 
Target Variable                  Churn

## Data Cleaning and Preparation

The following data quality checks and preparation steps were performed:
- Converted blank values in TotalCharges into Zeros as Tenure and accumulated charges are also zero.
- Converted appropriate columns to suitable data types.
- Checked and handled inconsistent whitespace in categorical variables.
- Investigated missing and unusual values.
- Performed outlier analysis on numerical variables including tenure, MonthlyCharges, and TotalCharges.
- Investigated potential inconsistencies between customer tenure, monthly charges, and total charges.
- Created additional engineered variables to investigate billing patterns.

# Exploratory Data Analysis

The analysis was structured into the following areas:
## 1. Customer Churn Distribution
Examined the overall distribution of churned and retained customers to understand the class balance of the target variable.
## 2. Customer Demographics and Churn
Analysed churn patterns across:
- Senior citizen status
- Partner status
- Dependents
Key observations showed that certain customer groups experienced noticeably higher churn rates.
## 3. Tenure and Churn
Investigated the relationship between customer tenure and churn.
The analysis showed that churned customers were strongly concentrated during the early stages of their customer relationship, particularly within the first few months.
## 4. Monthly Charges and Churn
Analysed the distribution of monthly charges across churned and retained customers.
Customers with higher monthly charges showed a stronger concentration of churn.
## 5. Services and Churn
Examined how customer churn varied across service-related variables, including:
- Internet service
- Online security
- Technical support
This analysis explored whether the availability or absence of specific services was associated with different churn patterns.
## 6. Contract and Tenure Analysis
Investigated the combined relationship between customer tenure, contract type, and churn to identify customer groups with higher retention risk.
## 7. Billing and Payment Behaviour
Explored the relationship between:
- Payment method
- Paperless billing
- Customer churn
This multivariate analysis helped identify billing and payment patterns associated with churn.

## Business Recommendations
Based on the exploratory findings, the company could consider:

- Strengthening early customer retention initiatives
- Focus on customers during their first months, when churn risk appears highest.
- Reviewing high monthly charge customer segments
- Investigate whether pricing, perceived value, or service satisfaction contributes to higher churn.
- Encouraging longer-term customer relationships
- Develop incentives that encourage customers to remain with the company for longer periods.
- Improving value-added service adoption
- Investigate whether services such as online security and technical support can contribute to improved customer retention.
- Developing targeted retention strategies
- Use customer characteristics, tenure, service subscriptions, and billing behaviour to identify higher-risk customer segments.

## Tools and Technologies

- Python
- Pandas — Data cleaning and manipulation
- NumPy — Numerical operations
- Matplotlib — Data visualization
- Seaborn — Statistical data visualization
- Google Colab - for analysis

## Project Structure
Customer-Churn-EDA/
│
├── data/
│   └── Telco-Customer-Churn.csv
│
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   └── EDA.ipynb
│
├── reports/
│   ├── Telco_customer_churn_data_cleaning_report.pdf
│   └── Telco_Churn_EDA_Executive_Report.pdf
│
└── README.md

## Project Objective
The objective of this project is to demonstrate an end-to-end exploratory data analysis workflow, including data cleaning, data quality investigation, univariate analysis, bivariate analysis, multivariate analysis, visualization, and business insight generation.
This project focuses on converting raw customer data into meaningful insights that could support customer retention strategies and further predictive modeling

## Author
Iqra Hayat
Aspiring Data Analyst
Linkedln : www.linkedin.com/in/iqra-hayat05
