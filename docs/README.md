Project Overview
This project aims to predict the ability of loan applicants to repay their loans using historical transaction and application data. By applying machine learning techniques to Home Credit's dataset, we intend to help the company ensure that clients capable of repayment are not rejected and that loans are provided with a principal, maturity, and repayment calendar that will empower clients to be successful.

Data Description
The data consists of two files:

application_train.csv: Training data with 307511 entries and 122 features, including a binary target variable.
application_test.csv: Test data with 48744 entries and 121 features.
Features
SK_ID_CURR: ID of loan in our sample.
TARGET: Target variable (1 for clients with payment difficulties, 0 otherwise).
NAME_CONTRACT_TYPE, CODE_GENDER, etc.: Descriptive attributes of applicants and loans.
Data Preparation
We performed the following steps to prepare the data:

Handling Missing Data: Identified and imputed missing values. Columns with more than 50% missing values were dropped.
Feature Encoding: Applied label encoding to categorical variables to convert them into a machine-readable form.
Feature Scaling: Standardized numerical features to have a mean of zero and a standard deviation of one.
Model Building
Several models were built to predict the target variable:

Logistic Regression: Provided a baseline for performance with an ROC-AUC of 0.60.
Decision Tree: Demonstrated overfitting with an ROC-AUC similar to Logistic Regression.
Random Forest: Improved prediction with an ROC-AUC of 0.71.
Gradient Boosting Machine (GBM): Achieved the best performance with an ROC-AUC of 0.75.
Evaluation
Models were evaluated based on accuracy and ROC-AUC scores. The Gradient Boosting Machine model showed the highest potential and was chosen for final predictions.

Results and Conclusion
The GBM model highlighted key predictors of default, such as EXT_SOURCE_2, EXT_SOURCE_3, and DAYS_BIRTH. Its performance was robust, making it suitable for deployment to predict loan repayment probabilities.
