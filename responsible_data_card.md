
# Responsible Data Card

## 1. Project Name
Credit Card Default Prediction Using Machine Learning

## 2. Dataset Source
UCI Machine Learning Repository – Default of Credit Card Clients Dataset.

Source:
https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients

## 3. Data Description
The dataset contains 30,000 customer records and 25 columns, including:
- Age
- Credit limit
- Payment history
- Bill amounts
- Previous payment amounts
- Default payment outcome

## 4. Data Provenance
The dataset is publicly available through the UCI Machine Learning Repository. It represents historical credit card customer data from Taiwan. The original collection context and documentation should be reviewed before use.

## 5. Consent and Usage
Public availability does not automatically mean unrestricted permission for every use. The dataset licence and usage conditions must be checked. The data should only be used for appropriate educational and research purposes.

## 6. Sensitive Attributes
The dataset contains demographic information such as:
- Sex
- Education
- Marital status
- Age

These attributes require special care. Fairness should be evaluated before using the model for financial decision support.

## 7. Missing Values
Initial dataset inspection found no missing values. Data types, unusual category values and duplicate records should still be checked before training.

## 8. Data Leakage Risks
Only information available before the prediction date should be used.
- Avoid using future payment information.
- Check the timing of repayment history columns.
- Do not include the target column as an input feature.
- Ensure training and testing data are separated properly.

## 9. Dataset Limitations
- The dataset represents a historical population in Taiwan.
- It may not represent customers in other countries.
- Historical patterns may not reflect current financial behaviour.
- The dataset may contain historical demographic biases.
- The default outcome distribution is imbalanced.

## 10. Responsible Data Usage
- Protect personal information.
- Restrict unnecessary data access.
- Check data quality.
- Evaluate fairness.
- Document limitations.
- Keep human review in important financial decisions.

## 11. Data Quality Summary
- Total records: 30,000
- Total columns: 25
- Missing values: 0
- Duplicate records: 0
- Default cases: 6,636
- Non-default cases: 23,364

## 12. Ethical Considerations
The model should support human decision-making rather than automatically reject customers. Predictions should be monitored for accuracy, fairness and reliability.