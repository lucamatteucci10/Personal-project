# Loan Default Prediction Project

## Contributors
- Luca Matteucci
- Santiago Mazzei
- Srithijaa Sankepally
- Victor Floriano

### 1.0 - Problem Statement:

The primary objective of this project is to predict customer default on loan payments. Through an analysis of the Lending Club Loan dataset, the goal is to create a model capable of predicting loan defaults and late payments. The intention is to enhance the lending process, diminish default risks, and improve profitability for lenders.

### 1.1 - Data Source:

We utilized the Lending Club Loan dataset, encompassing complete loan data issued from 2007 to 2015. This dataset originates from the Lending Club, a peer-to-peer lending company facilitating investment and borrowing interactions. The data includes borrower information, loan characteristics, and loan performance metrics. It can be accessed on Kaggle at [Lending Club Loan Dataset](https://www.kaggle.com/datasets/adarshsng/lending-club-loan-data-csv).

### 1.2 - Data Description:

The dataset encompasses approximately 2,260,668 observations and 145 variables (columns). Key variables include borrower characteristics (e.g., credit scores, income, employment details), loan specifics (e.g., loan amount, interest rate, purpose), and loan performance indicators (e.g., current loan status, delinquency history). Noteworthy variables for analysis include annual_inc, loan_amnt, int_rate, delinq_2yrs, purpose, among others.

The dataset comprises multiple data types, including float64 (105 instances), int64 (4 instances), and object (36 instances). Preprocessing requirements involve handling binary values ('Y'/'N') like hardship_flag, converting object columns to datetime (e.g., settlement_date), and managing text input variables (e.g., desc).

### 7 - Conclusion - Best model: XGboost

Following analysis of non-ensemble models, the best cross-validated F1 score performance on the Train set was achieved by XGboost with the following hyperparameters:

- n_estimators = 500
- learning_rate = 0.1
- gamma = 0

Therefore, XGBoost was chosen as the primary model and evaluated on the Test set. The model exhibited exceptional performance:

**XGBoost - Test:**

- Accuracy: 0.987
- Precision: 0.974
- Recall: 0.965
- F1: 0.969

Note: Despite marginally better performance by the Stacking Model, XGboost was selected due to its simplicity. Additionally, feature importances can be easily extracted from the XGboost model.
