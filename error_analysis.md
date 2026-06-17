```markdown id="err1"
# Error Analysis

## Overview
We analyze false positives and false negatives from the churn prediction model.


## False Positives (Predicted churn but did NOT churn)

### Business Risk
- Wasted retention cost
- Unnecessary marketing offers

### Customer Examples

- Customer ID: 1023  
  High inactivity but later made a purchase → misclassified as churn

- Customer ID: 1105  
  Low engagement period but still active customer

- Customer ID: 1188  
  Temporary drop in activity due to seasonal behavior

- Customer ID: 1210  
  Low web activity but high loyalty through repeat purchases

- Customer ID: 1333  
  Short-term inactivity but returned after campaign


## False Negatives (Predicted non-churn but DID churn)

### Business Risk
- Lost revenue
- Missed retention opportunity
- Customer lifetime value loss

### Customer Examples

- Customer ID: 1402  
  Gradual drop in frequency not captured early

- Customer ID: 1456  
  High historical value but sudden churn

- Customer ID: 1501  
  Support complaints increased before churn

- Customer ID: 1522  
  Refund rate increased but model missed signal

- Customer ID: 1600  
  Declining engagement across all channels

---

## Summary
False negatives are more critical than false positives because they represent missed churners and direct revenue loss.