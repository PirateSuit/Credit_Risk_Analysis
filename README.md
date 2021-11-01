# Credit Risk Analysis

## Purpose
The purpose of this analysis is to use different machine learning models on a dataset of credit cards to assess risk, and then to determine which, if any, of the models are strong enough to recommend to use for this purpose.

## Results

Here are the reports on how each machine learning model performed:

Random Oversample
![image](https://github.com/PirateSuit/Credit_Risk_Analysis/blob/main/images/random_oversample.png)

Smote
![image](https://github.com/PirateSuit/Credit_Risk_Analysis/blob/main/images/smote.png)

Cluster Centroids
![image](https://github.com/PirateSuit/Credit_Risk_Analysis/blob/main/images/cluster_centroids.png)

Smoteenn
![image](https://github.com/PirateSuit/Credit_Risk_Analysis/blob/main/images/smoteenn.png)

Balanced Random Forest
![image](https://github.com/PirateSuit/Credit_Risk_Analysis/blob/main/images/balanced_random_forest.png)

Easy Ensemble
![image](https://github.com/PirateSuit/Credit_Risk_Analysis/blob/main/images/easy_ensemble.png)

Ideally, one of our models would perfectly identify each high risk loans while also not falsely flagging low risk loans as high risk. We would also want the model to have a high accuracy and precision scores. Here are how the models performed on each of these tasks.

### Recall for High Risk
-Random Oversample: 62%
-Smote: 63%
-Cluster Centroids: 60%
-Smoteenn: 70%
-Balanced Random Forest: 67%
-Easy Ensemble: 91%

### Recall for Low Risk
-Random Oversample: 68%
-Smote: 66%
-Cluster Centroids: 43%
-Smoteenn: 57%
-Balanced Random Forest: 91%
-Easy Ensemble: 95%

### Accuracy
-Random Oversample: 65%
-Smote: 64%
-Cluster Centroids: 52%
-Smoteenn: 64%
-Balanced Random Forest: 79%
-Easy Ensemble: 93%

### Precision for High Risk
-Random Oversample: .01%
-Smote: .01%
-Cluster Centroids: .01%
-Smoteenn: .01%
-Balanced Random Forest: 04%
-Easy Ensemble: .08%

### Precision for Low Risk
-Random Oversample: 100%
-Smote: 100%
-Cluster Centroids: 100%
-Smoteenn: 100%
-Balanced Random Forest: 100%
-Easy Ensemble: 100%


## Summary

Among the models, recall of the loan risk is best assessed by the Easy Ensemble model, at 91% and 95% for high and low risk, respectively. It also is the standout on accuracy, sitting at 93%. However, when we look at the precision, there is a problem. No matter which model we used, the precision for low risk was at 100%, with high risk falling below 1%. This shows that any success the models are having at weeding out high risk loans comes at the cost of also incorrectly identifying a huge percentage of low risk loans as high risk. 

While this would allow a company to issue loans with a high degree of confidence in their safety, it would mean wrongly denying nearly all completely deserving customers of loans. No models are effective enough to be recommended.

All of the models manage to identify the low risk loans well

