# Credit Classification Project

## Objective
The objective of this project is to build a **Credit Classification Model** that predicts whether a credit applicant will have good or bad credit. This classification will help financial institutions assess risk before granting credit to customers.

## Dataset Description
The dataset contains information about applicants' financial history, employment details, and demographic information. The target variable is **'status'**, where:
- **0** represents good credit
- **1** represents bad credit

### Key Features:
- **Financial details**: Checking account balance, savings account balance, credit history, and amount borrowed.
- **Demographic details**: Age, marital status, and residence information.
- **Employment details**: Duration of employment and job category.
- **Credit behavior**: Loan duration, installment rate, and existing loan commitments.

## Data Preprocessing
To ensure accurate predictions, we performed several preprocessing steps:
- **Handling Missing Values**: Checked for missing values and handled them appropriately.
- **Encoding Categorical Variables**: Converted categorical variables into numerical format using one-hot encoding.
- **Feature Scaling**: Standardized numerical features to ensure uniformity in model training.

## Model Training and Evaluation
We implemented various machine learning models to classify credit status. The dataset was split into training and testing sets with an 80:20 ratio. Standardization was applied to improve model performance.

### Models Used and Accuracy:
1. **Logistic Regression** - 70%
2. **Ensemble Learning**:
   - **Voting Classifier** (Logistic Regression, KNN, Random Forest) - 71%
   - **Bagging Classifier** (Decision Tree as base estimator) - 72%
   - **AdaBoost Classifier** - **75% (Best Performing Model)**

## Conclusion
The **AdaBoost Classifier** achieved the highest accuracy of **75%**, making it the best model for predicting credit classification. This model improves prediction reliability by focusing more on difficult-to-classify instances.
