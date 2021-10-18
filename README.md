# Credit_Risk_Analysis

## Overview of the analysis
The purpose of this analysis was to use supervised machine learning techniques to train and evaluate unbalanced credit risk classification models using resampling. To predict credit risk, I used imbalanced-learn and scikit-learn libraries, along with oversampling, undersampling, combined sampling and bias-reducing classifier machine learning models. 


## Results
The balanced accuracy, precision and recall scores for each of the six machine learning models are listed below. 

### RandomOverSampler

Balanced Accuracy Score: 0.616

Precision: 0.99

Recall: 0.61

### SMOTE

Balanced Accuracy Score: 0.619

Precision: 0.99

Recall: 0.64

### ClusterCentroids

Balanced Accuracy Score: 0.507

Precision: 0.99

Recall: 0.43

### SMOTEEN

Balanced Accuracy Score: 0.639

Precision: 0.99

Recall: 0.57

### RandomForestClassifier

Balanced Accuracy Score: 0.657

Precision: 0.99

Recall: 1.00

### EasyEnsembleClassifier

Balanced Accuracy Score: 0.929

Precision: 0.99

Recall: 0.93

## Summary

Credit risk is an unbalanced data set, since a heavy majority of credit scores do not classify as high risk. To classify this unbalanced data set, I evaluated six machine learning models to identify which model produced the best accuracy, precision and recall using resampling and bias-reducing methods. 

All models had accuracy scores between 0.600 to 0.700, except for the EasyEnsembleClassifier, which had an accuracy score of 0.929. 

All six models had precision scores of 0.99, which meant that they were effectively classifying high risk credit out of all the data points. 

The highest recall score came from the RandomForestClassifier, with a recall of 1.00. This means that the RandomForestClassifier had the smallest relative amount of false negatives, which can be important because classifying a high-risk credit score as low-risk means that individual will not proactively work to lower their credit risk, which could mean risky loans.

Overall, the bias-reducing classifier models produced the highest accuracy, precision and recall scores, when compared to the resampling models. 

After examining the results, I would recommend using the EasyEnsembleClassifier model for predicting credit risk. The EasyEnsembleClassifier had the highest balanced accuracy score (0.929) paired with high precision (0.99) and recall (0.93) scores.
