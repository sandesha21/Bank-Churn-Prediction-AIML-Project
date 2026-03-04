# Project Requirements

## Background and Context

Businesses like banks that provide service have to worry about the problem of 'Churn' i.e. customers leaving and joining another service provider. It is important to understand which aspects of the service influence a customer's decision in this regard. Management can concentrate efforts on the improvement of service, keeping in mind these priorities.

## Objective

Given a Bank customer, build a neural network-based classifier that can determine whether they will leave or not in the next 6 months.

## Data Description

The case study is from an open-source dataset from Kaggle. The dataset contains 10,000 sample points with 12 distinct input features such as CreditScore, Geography, Gender, Age, Tenure, Balance, etc., plus a target variable (Exited).

## Data Dictionary

- **CustomerId**: Unique ID which is assigned to each customer
- **Surname**: Last name of the customer
- **CreditScore**: It defines the credit history of the customer
- **Geography**: A customer's location
- **Gender**: It defines the Gender of the customer
- **Age**: Age of the customer
- **Tenure**: Number of years for which the customer has been with the bank
- **NumOfProducts**: It refers to the number of products that a customer has purchased through the bank
- **Balance**: Account balance
- **HasCrCard**: It is a categorical variable that decides whether the customer has a credit card or not
- **EstimatedSalary**: Estimated salary
- **IsActiveMember**: It is a categorical variable that decides whether the customer is an active member of the bank or not (Active member in the sense, using bank products regularly, making transactions, etc)
- **Exited**: It is a categorical variable that decides whether the customer left the bank within six months or not. It can take two values:
  - `0` = No (Customer did not leave the bank)
  - `1` = Yes (Customer left the bank)

## Technical Requirements

### Model Requirements
- Build a neural network-based classifier
- Predict customer churn within 6-month timeframe
- Handle class imbalance in the dataset
- Optimize for business-relevant metrics (precision, recall, F1-score)

### Performance Expectations
- Achieve meaningful recall scores for churn detection
- Balance precision and recall for practical business application
- Provide model comparison and selection rationale
- Include business impact analysis

### Deliverables
1. Complete data preprocessing pipeline
2. Exploratory data analysis with insights
3. Multiple neural network model implementations
4. Model performance comparison and evaluation
5. Business impact analysis with financial metrics
6. Actionable recommendations for customer retention