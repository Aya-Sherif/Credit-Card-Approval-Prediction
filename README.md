
#  Credit Card Approval Prediction


## Dataset Overview

The dataset includes two tables:
1. **Client Information (Table 1)**: Contains details such as marital status, name, gender, family size, and annual income.
2. **Loan Payment History (Table 2)**: Tracks each client’s loan payment records.

## Project Workflow

### 1. Understanding the Dataset

### 2. Label Creation (Annotation)
Based on the loan payment history from Table 2, I assigned a label `{Good, Bad}` to each client:
- **Good (0)**: Includes clients with no major overdue payments or minor delays:
  - `0`: 1-29 days past due.
  - `C`: Paid off the loan that month.
  - `X`: No active loan for the month.
- **Bad (1)**: Includes clients with significant delays or defaults:
  - `1`: 30-59 days past due.
  - `2`: 60-89 days past due.
  - `3`: 90-119 days past due.
  - `4`: 120-149 days past due.
  - `5`: More than 150 days past due or written off.

### 3. Data Integration

### 4. Data Preprocessing
I performed the following preprocessing steps:
- **Data Cleaning**
- **Encoding**
- **Additional Preprocessing**: Applied normalization and scaling where necessary.

### 5. Modeling
I experimented with various supervised learning models:
- Random Forest
- Support Vector Machine (SVM)
- Logistic Regression

### 6. Hyperparameter Tuning
Utilized grid search and cross-validation to optimize the performance of each model.

### 7. Model Evaluation
Evaluated the models using:
- Confusion matrix
- Classification report (precision, recall, F1-score)
