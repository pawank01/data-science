# Credit Card Default Prediction Dashboard

## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Data Overview](#data-overview)
- [Dashboard Features](#dashboard-features)
- [Interactivity](#interactivity)
- [Model Evaluation](#model-evaluation)

### Project Overview
This interactive dashboard was developed to predict customer defaults based on their credit card transaction history. It includes multiple machine learning models: Decision Tree, Logistic Regression, and K-Nearest Neighbors (KNN). The dashboard provides visual insights and allows users to interactively input customer data to predict the likelihood of default.

### Key Features:
- Exploratory Data Analysis (EDA): Visual insights into demographic data and default patterns.
- Predictive Models: Implements Decision Tree, Logistic Regression, and KNN models, each with visualizations showing model performance and predictions.
- Interactive Dashboard: Users can input customer data to receive predictions from each of the models, simulating real-world scenarios.

### Data Overview
The dataset contains 30,000 observations related to customer credit card transactions. Key attributes include:
- LIMIT_BAL: Credit amount (in New Taiwan Dollars)
- SEX: Gender of the customer
- EDUCATION: Education level of the customer
- MARRIAGE: Marital status of the customer
- AGE: Age of the customer
- PAY_1 to PAY_6: Payment status for the previous six months
- BILL_AMT1 to BILL_AMT6: Bill amount for the past six months
- PAY_AMT1 to PAY_AMT6: Amount paid during the previous six months
- DEFAULT: Whether the customer defaulted (1) or not (0)

### Dashboard Features
#### 1. Customer Data Statistics
- Visualizations: Includes bar charts and line graphs that explore demographic data, such as age, gender, marital status, and education, in relation to default behavior.
- Statistics:
  - Total defaulters: 6,636 out of 30,000 customers.
  - Distributions based on gender, marital status, education, and age.
#### 2. Predictive Modeling
- Decision Tree Model: Visualizes key decision nodes that predict whether a customer will default based on payment history and bill amounts.
  - Model Accuracy: 82%
- Logistic Regression Model: Shows the ROC-AUC curve with an area of 0.717, indicating good performance in classifying defaults.
  - Model Accuracy: 82%
- K-Nearest Neighbors (KNN) Model: KNN assumes that similar data points exist closer. This model predicts defaults based on the proximity of new data points to the nearest neighbours.
  - Model Accuracy: 84% 
#### 3. User Input Panel
  - Interactive Inputs: Users can input values for key attributes (e.g., LIMIT_BAL, PAY_1, BILL_AMT1) to generate real-time predictions from each model. The models provide default predictions based on these inputs, simulating various credit card customer profiles.

### Interactivity
- Model Exploration: Visualizations for each model (Decision Tree, Logistic Regression, KNN) allow users to understand how the models function and their performance metrics.
- Prediction Simulation: Users can simulate different customer profiles by adjusting key attributes (e.g., credit limit, bill amounts, payment history) and observing the model predictions for default.

### Model Evaluation
- Decision Tree: Effective in showing critical decision nodes related to bill payments and payment history.
- Logistic Regression: Demonstrates strong classification capabilities, with good sensitivity and specificity, as depicted in the ROC-AUC curve.
- K-Nearest Neighbors (KNN): Provides accurate predictions based on proximity to similar data points, with an optimal number of 85 neighbours.
