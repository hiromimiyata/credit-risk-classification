# credit-risk-classification

# Credit Analysis Report

# Overview of the Analysis:
We are analyzing if the original data model or the resampled data model using RandomOverSampler to handle class imbalance is a good fit for building a model that can identify the creditworthiness of borrowers.

# Results:
The higher scores compared to each report are marked with an (*)

## Original Data Model:

- Accuracy Score: 99.2%

Classification Report:

- Precision Score (Label 0 - Healthy Loans): 100%

- Precision Score (Label 1 - High-Risk Loans): * 85%

- Recall Score (Label 0 - Healthy Loans): 99%

- Recall Score (Label 1 - High-Risk Loans): 91%

- F1-Score (Label 0 - Healthy Loans): 99%

- F1-Score (Label 1 - High-Risk Loans): 88%

- Support (Label 0 - Healthy Loans): 18,765

- Support (Label 1 - High-Risk Loans): 619

Confusion Matrix :

- True positives (label 1 correctly predicted as label 1) = 563

- True negatives (label 0 correctly predicted as label 0) = * 18663

- False positives (label 0 incorrectly predicted as label 1) = * 102

- False negatives (label 1 incorrectly predicted as label 0) = 56

## Resampled Data Model:

- Accuracy Score: * 99.4%

Classification Report:

- Precision Score (Label 0 - Healthy Loans): 100%

- Precision Score (Label 1 - High-Risk Loans): 84%

- Recall Score (Label 0 - Healthy Loans): 99%

- Recall Score (Label 1 - High-Risk Loans): * 99%

- F1-Score (Label 0 - Healthy Loans): 99%

- F1-Score (Label 1 - High-Risk Loans): * 91%

- Support (Label 0 - Healthy Loans): 18,765

- Support (Label 1 - High-Risk Loans): 619

Confusion Matrix :

- True positives (label 1 correctly predicted as label 1) = * 615

- True negatives (label 0 correctly predicted as label 0) = 18649

- False positives (label 0 incorrectly predicted as label 1) = 116

- False negatives (label 1 incorrectly predicted as label 0) = * 4

# Summary:

Both original and resampled data models are good at predicting the creditworthiness of customers. The resampled data model has a slightly better accuracy and recall score. The original data model has a higher precision score. The confusion matrix shows that the original data model is better at finding true negatives and has fewer false positives. The resampled data model has a higher true positive outcome and less false negatives. Based on these results, I recommend the resampled logistic regression model. It has better accuracy and better performance on high-risk loans which would be higher damage to the company if mispredicted. It also has good classification because of its high precision and recall values for high-risk and healthy loans. I do not recommend the original model because it has less accuracy overall, especially in the recall rate for high-risk loans. This causes a higher chance to miss risky loans. 
