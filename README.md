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
 
4. Complaint vs Churn

Insight: 
* Customers who complained are 3X more likely to churn
* Complain status is a strong churn signal

## Predictive Modeling

Model Used

* Logistoc Regression
* Binary classification (Churn / No Churn)

### Why Logistic Regression?
* Interpretable
* Probabilistic output
* Suitable for churn prediction problems


### Model Evaluation 
Confusion Matrix 

Interpretation (Business-Friendly): 

* True Negatives (945): Customers correctly predictly to stay
* False Positives (36): Customers predicted to churn but actually stayed
* False Negatives (113): Customers predicted to stay but churned
* True Positives (89): Customers correctly predictly to churn

The model performs well at identying non-churners, with room to improve recall for churners. 


## Churn Probabilty Ranking 
The model outputs churn probabilties, allowing customers to be ranking by risk. 
Example (Top High-Risk Customers)

CustomerID        Churn Probability
1682              0.943
860               0.935
3168              0.933
1942              0.908
488               0.904


### Key Business Insights
* Short customer tenure is a major churn indicatoe.
* Complaints dramatically increase churn risk.
* Inactivity after purchase is an early churn signal.
* Satisfaction scores may require validation.


## Recommendations
1. Early Retention Programs for new customers.
2. Complaint Resolution SLAs with churn alerts.
3. Proactive Re-engagement after last order inactivity.
4. Customer Risk Scoring embedded into CRM.
5. Survey Redesign to validate satisfaction scoring.

## Tools & Technologies
* SQL
* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

  
  





















   
























