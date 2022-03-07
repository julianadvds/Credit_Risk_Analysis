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
![Pic_1](https://github.com/julianadvds/Credit_Risk_Analysis/blob/main/Resources/Classification_report_RandomOversampling.png)

### SMOTE Oversampling
![Pic_2](https://github.com/julianadvds/Credit_Risk_Analysis/blob/main/Resources/Classification_report_SMOTEOversampling.png)

### Undersampling
![Pic_3](https://github.com/julianadvds/Credit_Risk_Analysis/blob/main/Resources/Classification_report_Undersampling.png)

### Combination (Over and Under) Sampling
![Pic_4](https://github.com/julianadvds/Credit_Risk_Analysis/blob/main/Resources/Classification_report_Combination(OverandUnder)Sampling.png)

### Balanced Random Forest Classifier
![Pic_5](https://github.com/julianadvds/Credit_Risk_Analysis/blob/main/Resources/Classification_report_BalancedRandomForestClassifier.png)

### Easy Ensemble AdaBoost Classifier
![Pic_6](https://github.com/julianadvds/Credit_Risk_Analysis/blob/main/Resources/Classification_report_EasyEnsembleAdaBoostClassifier.png)


## Summary

When reviewing the results table, it is clear to see that there is a big difference between the metrics used to evaluate the six machine model techniques.  From the table, it is also clear which model is is the most appropriate for assessing high-risk loans, the Easy Ensemble AdaBoost Classifier.  This model had a 91% accuracy while all other models were less than 80%.  The Easy Ensemble AdaBoost Classifier also had the highest precision, although the difference was only 0.04. This model also has the highest f1 score at 0.10 while most models were around 0.02. The final metric, recall, was a high 0.93, while the rest of the models were at 0.70 or less.  