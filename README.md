# Credit_Risk_Analysis

## Overview & Purpose
Evaluating large amounts of credit data tends to have unbalanced data, with a much larger portion being low risk compared to a small amount of high risk loans.  Using the existing data from Lending Club, a peer to peer serivce company, six different techniquies of supervised machine learning were applied to find the most effective model in prediction the outcome of future loans.  The model techniques included ways to over sample, undersample, use a combination of the two and reduce bias to find the best technique to evaluate the data. 

## Results
The results for the six machine learning models and their scores in balanced accuracy, recall and precision are as follows:

### Summary Table for "High Risk" Loans

| Technique | Accuracy  | Precision| Recall (Sensitivity) | F1 Score |
| ------------- | ------------- | ------------- | ------------- | ------------- |
|Naive Random Oversampling  | 65.73%  | 0.01  | 0.71  | 0.02  |
| SMOTE Oversampling  | 66.22%  | 0.01  | 0.63  | 0.02  |
| Undersampling  | 66.22%  | 0.01  |  0.69 | 0.01  |
| Combination (Over and Under) Sampling | 54.74%  | 0.01  | 0.80  | 0.02  |
| Balanced Random Forest Classifier  | 78.85%  | 0.03  | 0.70  | 0.06  |
| Easy Ensemble AdaBoost Classifier  | 91.54%  | 0.05  | 0.93  |  0.10 |

### Naive Random Oversampling