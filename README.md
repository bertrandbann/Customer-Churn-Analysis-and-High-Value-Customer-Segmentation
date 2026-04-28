# Customer Churn Analysis & High-Value Customer Segmentation

## Executive Summary
This project analyses customer churn behaviour within the telecommunications industry using Python, statistical modelling, and customer segmentation techniques. The analysis combines exploratory data analysis, feature engineering, and logistic regression modelling to identify the main drivers of churn and detect high-value customers with strong retention potential.

The project achieved approximately **80% prediction accuracy** with an **AUC score of 0.84**, demonstrating strong predictive capability for identifying customers at risk of leaving. The findings provide actionable business insights that can support customer retention strategies, revenue protection, pricing optimisation, and customer lifetime value management.

---

# Business Problem
Customer churn is one of the largest challenges faced by subscription-based businesses such as telecommunications providers. Losing customers increases acquisition costs, reduces recurring revenue, and negatively impacts long-term profitability.

The objective of this project was to:

- Identify the key factors driving customer churn
- Predict customers most likely to leave
- Detect high-value customers with strong retention value
- Provide business recommendations to improve customer retention and reduce revenue leakage

---

# Project Objectives

- Perform exploratory data analysis on customer behaviour
- Clean and preprocess customer data for modelling
- Build a logistic regression model to predict churn probability
- Evaluate model performance using classification metrics
- Analyse business drivers behind churn behaviour
- Segment high-value customers based on service usage and tenure
- Translate statistical findings into business-focused recommendations

---

# Dataset Overview
The dataset contains customer-level information from a telecommunications company, including:

- Customer demographics
- Contract information
- Internet and phone services
- Billing and payment methods
- Monthly and total charges
- Customer tenure
- Churn status

### Example Variables

| Variable | Description |
|---|---|
| tenure | Number of months the customer stayed with the company |
| MonthlyCharges | Monthly subscription charges |
| TotalCharges | Total lifetime revenue generated |
| Contract | Type of customer contract |
| PaymentMethod | Customer payment method |
| TechSupport | Whether technical support is subscribed |
| OnlineSecurity | Whether online security services are active |
| Churn | Whether the customer left the company |

---

# Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Scikit-learn
- Jupyter Notebook

---

# Project Workflow

## 1. Data Cleaning & Preparation

Several preprocessing steps were performed to improve data quality and modelling reliability:

- Converted `TotalCharges` into numeric format
- Removed inconsistent categorical labels
- Dropped unnecessary identifiers
- Created dummy variables for categorical features
- Managed missing values using median imputation
- Engineered additional behavioural variables

### Feature Engineering

A custom feature called `num_services` was created to estimate overall customer engagement based on subscribed services.

This helped identify:

- Highly engaged customers
- Customers with stronger product adoption
- Potential high-value customer segments

---

## 2. Exploratory Data Analysis

Exploratory analysis was conducted to understand customer behaviour patterns and churn trends.

### Key Findings

- Customers with longer tenure were significantly less likely to churn
- Customers on monthly contracts showed higher churn risk
- Higher monthly charges were associated with increased churn probability
- Customers subscribed to support and security services showed lower churn behaviour
- Electronic check payment users displayed elevated churn rates

---

# Logistic Regression Modelling

## Why Logistic Regression?

Logistic regression was selected because the target variable (`Churn`) is binary and the model provides strong interpretability for business decision-making.

The model estimates the probability that a customer will churn based on behavioural and financial characteristics.

---

## Model Performance

| Metric | Result |
|---|---|
| Accuracy | ~80% |
| AUC Score | ~0.84 |
| Pseudo R² | ~0.27 |

### Interpretation

The model demonstrated strong predictive performance and good discrimination between churn and non-churn customers.

The AUC score of approximately **0.84** indicates that the model can effectively distinguish customers likely to leave from those likely to remain.

---

# Model Evaluation

## Classification Performance

| Class | Precision | Recall | F1-Score |
|---|---|---|---|
| Non-Churn | 0.84 | 0.90 | 0.87 |
| Churn | 0.64 | 0.53 | 0.58 |

### Business Interpretation

- The model performs strongly in identifying retained customers
- Churn prediction remains more challenging due to behavioural complexity
- The model can still support proactive retention campaigns by identifying high-risk customer groups

---

# Key Churn Drivers

## Factors Reducing Churn

### Contract Commitment
Customers on one-year and two-year contracts showed significantly lower churn probability.

### Service Engagement
Customers using additional services such as:

- Online Security
- Tech Support
- Device Protection

were more likely to remain with the company.

### Customer Tenure
Long-term customers demonstrated higher loyalty and lower churn behaviour.

---

## Factors Increasing Churn

### High Monthly Charges
Customers with higher monthly bills showed greater churn risk, suggesting increased price sensitivity.

### Monthly Contracts
Customers on month-to-month plans displayed substantially higher churn behaviour compared to long-term contract customers.

### Electronic Check Payments
Electronic check users were associated with elevated churn probability, potentially indicating lower customer engagement or satisfaction.

---

# High-Value Customer Segmentation

## Definition of High-Value Customers

High-value customers were identified using:

- Above-average tenure
- Above-average number of subscribed services
- High total revenue contribution
- Lower churn probability

---

## Characteristics of High-Value Customers

| Metric | Approximate Value |
|---|---|
| Average Tenure | ~60 Months |
| Average Monthly Charges | ~£95 |
| Average Total Charges | Significantly Above Dataset Average |

### Business Interpretation

These customers generate strong recurring revenue and demonstrate higher product adoption and retention.

Protecting these customers should be prioritised through:

- Loyalty programs
- Personalised offers
- Premium customer support
- Long-term contract incentives

---

# Business Recommendations

## 1. Improve Retention for Month-to-Month Customers

Introduce incentives encouraging migration toward longer-term contracts.

Examples:

- Bundled discounts
- Loyalty rewards
- Contract upgrade offers

---

## 2. Expand Value-Added Services

Customers subscribed to support and security services demonstrated lower churn behaviour.

The company could:

- Promote bundled service packages
- Upsell protection services
- Offer free trials for support services

---

## 3. Monitor High Monthly Charges

High monthly pricing increased churn probability.

Potential actions:

- Pricing reviews
- Flexible subscription plans
- Retention discounts for at-risk customers

---

## 4. Develop Predictive Retention Campaigns

The churn prediction model can support:

- Early churn detection
- Personalised retention campaigns
- Revenue protection strategies
- Customer lifetime value optimisation

---

# Business Impact

This project demonstrates how statistical modelling and customer analytics can support strategic business decisions.

Potential applications include:

- Customer retention optimisation
- Revenue forecasting
- Marketing segmentation
- Churn prevention strategies
- Customer lifetime value management
- Targeted promotional campaigns

---

# Key Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Customer Analytics
- Predictive Modelling
- Logistic Regression
- Feature Engineering
- Classification Modelling
- Business Intelligence Storytelling
- Statistical Interpretation
- Customer Segmentation
- Business Recommendation Development

---

# Future Improvements

Potential future enhancements include:

- Random Forest and XGBoost modelling
- Hyperparameter optimisation
- Churn probability dashboards in Power BI
- Customer lifetime value modelling
- Time-series customer behaviour analysis
- Real-time churn monitoring systems

---

# Conclusion

This project demonstrates how data analytics and predictive modelling can be used to identify churn behaviour, understand customer risk factors, and support retention-focused business decisions.

By combining statistical modelling with business interpretation, the analysis provides a practical framework for reducing churn, protecting revenue, and identifying high-value customers.

The project highlights the importance of transforming raw customer data into actionable business intelligence capable of supporting operational and strategic decision-making.

---

# Author

## Bertrand Bann

GitHub: https://github.com/bertrandbann
