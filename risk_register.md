# Risk Register

## Project: Credit Card Default Prediction Using Machine Learning

| No. | Risk | Impact | Mitigation |
|---|---|---|---|
| 1 | Biased predictions | Unfair treatment of customers | Check fairness across groups |
| 2 | Missing data | Incorrect predictions | Identify and handle missing values |
| 3 | Data leakage | Misleading model performance | Use only information available before prediction |
| 4 | Privacy issues | Misuse of customer information | Protect sensitive data |
| 5 | Model drift | Model performance decreases over time | Monitor model performance regularly |
| 6 | False positive | Reliable customers may be flagged | Use human review |
| 7 | False negative | High-risk customers may be missed | Evaluate recall and error costs |
| 8 | Incorrect decisions | Financial or customer harm | Allow human intervention and rollback |
| 9 | Uncertain predictions | Unreliable decisions | Abstain and send cases for manual review |
| 10 | Data quality changes | Reduced prediction reliability | Monitor data quality and investigate changes |

## Monitoring Plan

- Monitor model performance regularly.
- Review false positives and false negatives.
- Check for unfair outcomes across customer groups.
- Investigate changes in data quality.
- Monitor prediction confidence and data drift.

## Human Review

Uncertain predictions should be sent to a qualified human reviewer. The model should support decision-making and should not independently reject customers.

## Rollback Plan

If the model becomes unreliable or causes unacceptable harm:

- Stop using model predictions.
- Return to existing business rules.
- Investigate the cause of failure.
- Review the model before considering future use.

## Rollback Conditions

- Significant decline in model performance.
- Evidence of unfair predictions.
- Unexpected changes in input data.
- Unacceptable false-positive or false-negative rates.
- Privacy or data security concerns.

## Conclusion

The risks must be reviewed and controlled before any real-world deployment. Human supervision, regular monitoring and a rollback plan are essential for responsible machine learning.