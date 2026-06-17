# Model Card: Customer Churn Prediction


## Model Name
Customer Churn Prediction Model (60-day horizon)


## Intended Use
- Identify customers likely to churn
- Support retention campaigns
- Prioritize high-risk customers for intervention


## Data Used
- Customer demographics
- Order history (RFM features)
- Support tickets
- Refund behavior
- Web/app activity
- Campaign interactions


## Model Type
- Baseline: Logistic Regression
- Final Model: Random Forest Classifier


## Performance

- Accuracy: ~ (from metrics.json)
- Precision: ~
- Recall: ~
- F1-score: ~
- ROC-AUC: ~

Threshold used: 0.40


## Key Features
- Recency
- Frequency
- Monetary value
- Ticket count
- Refund rate
- Web activity
- Campaign engagement


## Limitations
- Behavior may change over time
- External factors not included
- Cold-start customers may have weak predictions


## Ethical Considerations
- Predictions may lead to targeted marketing
- Incorrect predictions may affect customer experience
- Model should support decisions, not replace human judgment


## Monitoring
- Model drift
- Feature distribution changes
- Drop in recall for churners
- Regular retraining required


## When NOT to use
- Without updated data
- For legal/automated high-stakes decisions
- Without human validation