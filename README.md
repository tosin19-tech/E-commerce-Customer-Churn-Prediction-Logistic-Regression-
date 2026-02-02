# E-commerce-Customer-Churn-Prediction-Logistic-Regression-

## Project Overview
Customer churn directly impacts revenue growth in e-commerce businesses. This project build a logistic regression model to predict the probability that a customer will churn, 
using behavioral, transactional, and service-related features. 
The goal is not just prediction, but decision support: 
* Identify customers at high risk of churn
* Understand why customers churn
* Provide actionable business recommendations

## Business Problem 
The business wants to answer three key questions: 
1. Which customers are most likely to churn?
2. What factors drive churn behavior?
3. How can the business proactively reduce churn?

## Dataset Description
The dataset represents customer-level e-commerce activity. 

Target Variiable 
* Churn (0 = Stayed = 0, 1 = Churned)

  Key Features Used

* Tenure - How long the customer has been with the company
* WarehouseToHome - Distance between warehouse and customer
* NumberofDeviceRegistered
* SatisfactionScore
* Complaint (0 = No, 1 = Yes)
* DaySinceLastOrder

A unique Customer ID was added to support customer-level churn ranking. 


## Exploratory & Diagnostic Analysis
Before modeling exploratory analysis was performed to understand churn behavior. 

1. Tenure Distribution by Churn Status

Insight: 
* Customers who tend to have shorter tenure
* Long-tenure customers are significantly more likelty to stay


2. Days Since Last Order by Churn Status

Insight:
* Churned customers typically stop ordering soon after their last purchase
* Long inactivity is less common but still present

3. Churn Rate by Satisfaction Score

Insight: 
* Higher satisfaction scores unexpectedly show higher churn rates
* This suggests potential issues such as:
  - Survey scale reversal
  - Post-purchase dissatisfaction
  - Incentivized but disengaged customers
   
























