# Credit Risk Analysis

## Overview of the loan prediction risk analysis

### Purpose

The purpose of this analysis is to use machine learning to predict credit risk. The data used for this analysis is from LendingClub, a peer-to-peer lending services company. The data is from 2007 to 2019. The data is imbalanced, with high risk loans making up only 2% of the data. The goal is to use machine learning to train and evaluate models with unbalanced classes. The models will be used to predict credit risk.

### Results

#### Resampling Models to Predict Credit Risk

Using my knowledge of the `imbalanced-learn` and `scikit-learn` libraries, I evaluated three machine learning models by using resampling to determine which is better at predicting credit risk.

Using these algorithms, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix, and a classification report.

I compared two ensemble algorithms to determine which algorithm results in the best performance. I trained a `Balanced Random Forest` Classifier and an `Easy Ensemble AdaBoost` classifier.

The results of this portion of the analysis are as follows:

- The balanced accuracy score for the `BalancedRandomForestClassifier` random oversampling model is `0.9940714908456844`.

The confusion matrix for the random oversampling model is as follows:

![Random Oversampling Confusion Matrix]()

he classification report for the random oversampling model is as follows:

![Random Oversampling Classification Report]()

- The balanced accuracy score for the `EasyEnsembleClassifier` is `0.5`.

The confusion matrix for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Confusion Matrix]()

The classification report for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Classification Report]()

#### Use of SMOTEENN algorithm to Predict Credit Risk

Using my already created training  and target variables, I used a combinatorial approach of `over- and undersampling` with the `SMOTEENN` algorithm to determine if the results from the combinatorial approach were better at predicting credit risk than the resampling algorithms from my resampling models.

Using the SMOTEEN algorithm, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix and a classification report.

The results of this portion of the analysis are as follows:

- The balanced accuracy score for the SMOTEENN combination sampling model is 1.0.

- The confusion matrix for the SMOTEENN combination sampling model is as follows:

![SMOTEENN Confusion Matrix]()

- The classification report for the SMOTEENN combination sampling model is as follows:

![SMOTEENN Classification Report]()


#### Ensemble Classifiers to Predict Credit Risk

Continuing to use my knowledge of the `imbalanced-learn` library, I trainied and compared two differen ensemble classifiers to predict credit risk and evaluate each model. `

The first ensemble classifier I used was the `BalancedRandomForestClassifier` and the second was the `EasyEnsembleClassifier`.

Similar to the previous models, I resampled the dataset, viewed the count of the target classes, trained the ensemble classifier, calculated the balanced accuracy score, and finally, generated both a confusion matrix and a classification report.

The results of this portion of the analysis are as follows:

#### Balanced Random Forest Classifier
- The balanced accuracy score for the `BalancedRandomForestClassifier` is `0.9949433304272014`.

- The confusion matrix for the `BalancedRandomForestClassifier` is as follows:

![Balanced Random Forest Confusion Matrix]()

- The classification report for the `BalancedRandomForestClassifier` is as follows:

![Balanced Random Forest Classification Report]()

#### Easy Ensemble AdaBoost Classifier
- The balanced accuracy score for the `EasyEnsembleClassifier` is `0.9446672478930543`.

- The confusion matrix for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Confusion Matrix]()

- The classification report for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Classification Report]()



### Summary

The easy ensemble classifier model has the highest balanced accuracy score of 0.93. This model is the best model for predicting credit risk.

## Resources

- Data Source: LoanStats_2019Q1.csv
- Software: Python 3.7.6, Jupyter Notebook 6.0.3

## Results

### Random Oversampling

The balanced accuracy score for the random oversampling model is 0.65. The confusion matrix for the random oversampling model is as follows:

![Random Oversampling Confusion Matrix]()

The classification report for the random oversampling model is as follows:

![Random Oversampling Classification Report]()

### SMOTE Oversampling

The balanced accuracy score for the SMOTE oversampling model is 0.66. The confusion matrix for the SMOTE oversampling model is as follows:

![SMOTE Oversampling Confusion Matrix]()

The classification report for the SMOTE oversampling model is as follows:

![SMOTE Oversampling Classification Report]()
