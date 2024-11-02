# Customer Churn Prediction with Naive Bayes

## Project Overview

The goal of this project is to build and test a Naive Bayes model that predicts customer churn based on banking data. Churn is defined as customers who have left the bank. By predicting churn, the bank can take proactive measures, such as offering promotions or discounts, to retain customers.

The target variable in this project is **Exited**, which is a Boolean indicator where:
- `0` means the customer did not leave the bank
- `1` means the customer left the bank

This classification task uses the **Gaussian Naive Bayes** model from `scikit-learn`, which assumes continuous predictor variables with a normal distribution. While our data may not perfectly align with this assumption, GaussianNB is often effective in practical applications.

## Data Dictionary

| Column Name     | Type  | Description                                                         |
|-----------------|-------|---------------------------------------------------------------------|
| `Exited`        | int   | Target variable: 0 if the customer stayed, 1 if they left          |
| `Age`           | int   | Age of the customer                                                |
| `Balance`       | float | Balance amount in the customer's bank account                      |
| `NumOfProducts` | int   | Number of bank products held by the customer                       |
| `CreditScore`   | int   | Credit score of the customer                                       |
| `Gender`        | object| Gender of the customer                                             |
| `Tenure`        | int   | Number of years the customer has been with the bank                |
| `Geography`     | object| Customer's location                                                |
| `IsActiveMember`| int   | 1 if the customer is an active member, 0 otherwise                 |
| `EstimatedSalary` | float | Estimated annual salary of the customer                        |

**Let's explore the power of probabilistic classification!**
