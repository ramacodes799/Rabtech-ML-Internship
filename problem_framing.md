# ML Problem Framing Memo

## Project Title
Credit Card Default Prediction Using Machine Learning

## 1. Problem Statement
Financial institutions need to identify credit card customers who may fail to make their next month's payment. This project explores how machine learning can help predict credit card default risk.

## 2. Business Decision
Identify credit card accounts that require additional human review.

## 3. Prediction Target
Predict whether a customer will default on the next month's payment using the target column `default payment next month`.

## 4. Unit of Observation
One customer represents one observation (one row in the dataset).

## 5. Action Window
Predictions should be made before the next month's payment decision, using only information available at that time.

## 6. Non-ML Baseline
Use existing business rules and historical repayment information to assess customer risk.

## 7. Why Machine Learning?
Machine learning may identify patterns in repayment history, credit limits, bills and payment amounts that simple business rules cannot easily detect.

## 8. Business Metrics
- Reduce missed high-risk cases.
- Avoid unnecessarily flagging reliable customers.
- Support consistent human review.

## 9. Responsible AI Considerations
- Protect customer privacy.
- Check for bias in sensitive attributes.
- Prevent data leakage.
- Use human review for uncertain predictions.
- Monitor model performance.

## 10. Expected Outcome
Evaluate whether machine learning can improve credit card default risk assessment compared with existing business rules without creating unacceptable risks.

## 11. False Positive and False Negative Costs
- False Positive: A customer who would pay is incorrectly flagged for review, causing unnecessary delays.
- False Negative: A customer who defaults is incorrectly predicted as non-default, increasing financial risk.

## 12. Model Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## 13. Abstention and Human Review
- Send uncertain predictions for manual review.
- Do not automatically reject customers based on model predictions.
- Keep final decisions under human supervision.

## 14. Monitoring and Rollback
- Monitor model performance regularly.
- Check for changes in customer data patterns.
- Monitor fairness across customer groups.
- Stop using the model if performance becomes unreliable.
- Return to existing business rules if the model fails.