# deep-learning-challenge

# Overview of the Analysis:
We are analyzing if the original data model or the resampled data model using RandomOverSampler to handle class imbalance is a good fit for building a model that can identify the creditworthiness of borrowers.

# Results:
The higher scores compared to each report are marked with an (*)

## Original Data Model:

Classification Report:

Accuracy Score: 99.2%

Precision Score (Label 0 - Healthy Loans): 100%

Precision Score (Label 1 - High-Risk Loans): * 85%

Recall Score (Label 0 - Healthy Loans): 99%

Recall Score (Label 1 - High-Risk Loans): 91%

F1-Score (Label 0 - Healthy Loans): 99%

F1-Score (Label 1 - High-Risk Loans): 88%

Support (Label 0 - Healthy Loans): 18,765

Support (Label 1 - High-Risk Loans): 619

## Resampled Data Model:

Classification Report:

Accuracy Score: 99.4%

Precision Score (Label 0 - Healthy Loans): 100%

Precision Score (Label 1 - High-Risk Loans): 84%

Recall Score (Label 0 - Healthy Loans): 99%

Recall Score (Label 1 - High-Risk Loans): * 99%

F1-Score (Label 0 - Healthy Loans): 99%

F1-Score (Label 1 - High-Risk Loans): * 91%

Support (Label 0 - Healthy Loans): 18,765

Support (Label 1 - High-Risk Loans): 619

# Summary:

Both original and resampled data models are good at predicting the creditworthiness of customers. The resampled data model has a slightly better accuracy and recall score. The original data model has a higher precision score.
