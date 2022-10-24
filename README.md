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

![Random Oversampling Confusion Matrix](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/Random%20Oversampling%20Confusion%20Matrix.png)

he classification report for the random oversampling model is as follows:

![Random Oversampling Classification Report](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/Random%20Oversampling%20Classification%20Report.png)

- The balanced accuracy score for the `EasyEnsembleClassifier` is `0.5`.

The confusion matrix for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Confusion Matrix](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/EasyEnsembleClassifier%20Confusion%20Matrix.png)

The classification report for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Classification Report](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/EasyEnsembleClassifier%20Classification%20Report.png)

#### Use of SMOTEENN algorithm to Predict Credit Risk

Using my already created training  and target variables, I used a combinatorial approach of `over- and undersampling` with the `SMOTEENN` algorithm to determine if the results from the combinatorial approach were better at predicting credit risk than the resampling algorithms from my resampling models.

Using the SMOTEEN algorithm, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix and a classification report.

The results of this portion of the analysis are as follows:

- The balanced accuracy score for the SMOTEENN combination sampling model is 1.0.

- The confusion matrix for the SMOTEENN combination sampling model is as follows:

![SMOTEENN Confusion Matrix](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEEN%20Confusion%20Matrix.png)

- The classification report for the SMOTEENN combination sampling model is as follows:

![SMOTEENN Classification Report](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEEN%20Classification%20Report.png)

#### Ensemble Classifiers to Predict Credit Risk

Continuing to use my knowledge of the `imbalanced-learn` library, I trainied and compared two differen ensemble classifiers to predict credit risk and evaluate each model. `

The first ensemble classifier I used was the `BalancedRandomForestClassifier` and the second was the `EasyEnsembleClassifier`.

Similar to the previous models, I resampled the dataset, viewed the count of the target classes, trained the ensemble classifier, calculated the balanced accuracy score, and finally, generated both a confusion matrix and a classification report.

The results of this portion of the analysis are as follows:

#### Balanced Random Forest Classifier

- The balanced accuracy score for the `BalancedRandomForestClassifier` is `0.9949433304272014`.

- The confusion matrix for the `BalancedRandomForestClassifier` is as follows:

![Balanced Random Forest Confusion Matrix](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/Balanced%20Random%20Forest%20Classifier%20Confusion%20Matrix.png)

- The classification report for the `BalancedRandomForestClassifier` is as follows:

![Balanced Random Forest Classification Report](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/Balanced%20Random%20Forest%20Classifier%20Classification%20Report.png)

#### Easy Ensemble AdaBoost Classifier

- The balanced accuracy score for the `EasyEnsembleClassifier` is `0.9446672478930543`.

- The confusion matrix for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Confusion Matrix](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/EasyEnsembleClassifier%20Confusion%20Matrix%202.png)

- The classification report for the `EasyEnsembleClassifier` is as follows:

![Easy Ensemble Classification Report](https://github.com/hastyjr/Credit_Risk_Analysis/blob/main/Resources/images/EasyEnsembleClassifier%20Confusion%20Matrix.png)

### Summary

The results of the analysis show that the `SMOTEENN` algorithm is the best model for predicting credit risk. The `SMOTEENN` algorithm has a balanced accuracy score of 1.0, which is the highest of all the models tested in this analysis.

The `SMOTEENN` algorithm also has the highest 

- `recall score` of all the models, which is 1.0.

- `geometric mean score` of all the models, which is 1.0.

- `f1 score` of all the models, which is 1.0.

- `support score` of all the models, which is 1.0.

- `precision score` of all the models, which is 1.0.

- `average precision score` of all the models, which is 1.0.

- `average recall score` of all the models, which is 1.0.

- `average f1 score` of all the models, which is 1.0.

- `average support score` of all the models, which is 1.0.

