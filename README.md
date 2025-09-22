# PROJECT BACKGROUND
Credit risk assessment is a crucial part of the financial services industry. Banks and lending institutions need to determine whether a loan applicant is a good risk or a bad risk. Traditionally, this is done through manual evaluation of demographic, financial, and behavioral factors.
In this project, a dataset from Kaggle was used to build a machine learning model that predicts credit risk based on multiple applicant attributes such as age, financial history, and loan-related details.

# DATA STRUCTURE AND INITIAL CHECKS
## DATA STRUCTURE
The dataset includes the following key columns:
Age -> Age of the applicant.
Sex –> Gender of the applicant.
Income Sources –> Number of income streams (e.g., salary, business, investments).
Housing –> Housing status (own, rent, free).
Savings Account –> Balance in savings account.
Chequing Account –> Balance in current account.
Credit Amount –> Loan amount requested.
Duration –> Duration of the loan (in months).
Purpose –> Purpose of the loan (car, education, furniture, etc.).
Risk (Target Variable) –> Whether the applicant is a good risk (1) or bad risk (0).

# INITIAL DATA CHECKS 
- Checked for missing values and handled them appropriately.
- Converted categorical variables (e.g., housing, purpose, sex) into numeric form using encoding techniques.
- Verified class balance in the target variable (good vs. bad risk).

# EXECUTIVE SUMMARY
The project workflow involved the following steps:
1. Data Understanding & Cleaning – Performed exploratory data analysis (EDA), identified missing values, and standardized categorical and numerical variables.
2. Feature Engineering – Encoded categorical features and normalized numeric features for better model performance.
3. Model Selection – Tested multiple machine learning models (e.g., Decision Tree, Random Forest, XGBoost) to predict risk.
4. Training & Validation – Split the dataset into training and testing sets to evaluate performance.
5. Hyperparameter Tuning – Used grid search/random search to optimize model parameters.

# MODEL PERFORMANCE
1. Decision Tree Classifier
   - Best parameters -> max_depth=7, min_samples_leaf=1, min_samples_split=2
   - Accuracy -> 0.72

2. Random Forest Classifier
   - Best parameters -> max_depth=7, n_estimators=100
   - Accuracy -> 0.77
  
3. XGboost Classifier
   - Best parameters -> max_depth=7, n_estimators=100
   - Accuracy -> 0.72

# INSIGHTS :
- Features such as credit amount, savings account balance, and duration were strong predictors of credit risk.
- Demographic factors like age and sex also contributed but had less predictive power compared to financial attributes.
- The model shows strong potential for use in credit risk screening systems, assisting banks in making data-driven lending decisions.
