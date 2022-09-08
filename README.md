# Credit Risk Analysis

## Purpose

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques to train and evaluate models are used with unbalanced classes. Imbalanced-learn and scjkit-learn libraries are used to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, oversampling of the data is done using Random OverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. A combinatorial approach of over- and undersampling using the SMOTEENN algorithm is used as well. Then the two new machine learning models that reduce bias are compared, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Overview

Various libraries and algorithms are used in this project:

•	Imbalanced-learn

•	Scikit-learn

•	RandomOverSampler

•	SMOTE algorithms

•	ClusterCentroids algorithm

•	SMOTEENN algorithm

•	BalancedRandomForestClassifier (bias reduction model)

•	EasyEnsembleClassifier (bias reduction model)

Processes used in this projects:


•	Use Machine Learning algorithms in data analytics

•	Create training and test groups from a given data set.

•	Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.

•	Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.

•	Compare the advantages and disadvantages of each supervised learning algorithm.

•	Determine which supervised learning algorithm is best used for a given data set or scenario.

•	Use ensemble and resampling techniques to improve model performance.

## Results

The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores are listed below:

### Naïve Random Oversampling

![Naive_random_oversampling](https://user-images.githubusercontent.com/103263248/188501568-a9238da2-8b0e-4760-9ffa-6e5f8a9cb1b1.png)

•	Balanced Accuracy: 0.6515938052705158

•	Precision: The precision is low for High-risk loans and is high for Low-risk loans.

•	Recall: High-risk = 0.62

•	Recall: Low-risk = 0.68

### SMOTE Oversampling

![SMOTE_oversampling](https://user-images.githubusercontent.com/103263248/188501577-ab1f3110-344d-4f13-833a-a0ceec85531a.png)

•	Balanced Accuracy: 0.6241876870888075

•	Precision: The precision is low for High-risk loans and is high for Low-risk loans.

•	Recall: High-risk = 0.59

•	Recall: Low-risk = 0.66

### Undersampling

![undersampling](https://user-images.githubusercontent.com/103263248/189012437-e8a323d9-8c9a-4511-9101-51b0f072de17.png)

•	Balanced Accuracy: 0.5160196365189295

•	Precision: The precision is low for High-risk loans and is high for Low-risk loans.

•	Recall: High-risk = 0.60

•	Recall: Low-risk = 0.43

### Combination Over-Under Sampling

![combination_over_and_under_sampling](https://user-images.githubusercontent.com/103263248/188501597-c3292497-eaab-42b6-b110-81951e31e2f7.png)

•	Balanced Accuracy: 0.6384588112533288

•	Precision: The precision is low for High-risk loans and is high for Low-risk loans.

•	Recall: High-risk = 0.70

•	Recall: Low-risk = 0.58

### Balanced Random Forest Classifier

![balanced_random_forest_classifier](https://user-images.githubusercontent.com/103263248/188501625-a2097aa4-a553-4c21-9696-98ebe8abdfa2.png)

•	Balanced Accuracy: 0.7877672625306695

•	Precision: The precision is low for High-risk loans and is high for Low-risk loans.

•	Recall: High-risk = 0.67

•	Recall: Low-risk = 0.91

### Easy Ensemble AdaBoost Classifier

![easy_ensemble_adaboost_classifier](https://user-images.githubusercontent.com/103263248/188501640-43653ca0-0fe5-42e5-bfaa-6a9bb77c3905.png)

•	Balanced Accuracy: 0.925427358175101

•	Precision: The precision is low for High-risk loans and is high for Low-risk loans.

•	Recall: High-risk = 0.91

•	Recall: Low-risk = 0.94

## Summary

When working with balanced accuracy, the highest compared accuracy between 0 and 1, and how close it is to 1 will be the best choice of machine learning model. The best model to chose for the credit card dataset is the Easy Ensemble AdaBoost Classifier model which had a balanced accuracy of 0.93. The precision for the models were within appropriate range and similar in their results of low precision for High-risk loans and high precision for Low-risk loans. The recall score also needs to land between 0 and 1, with the numbers closest to 1 being the best model. The Easy Ensemble AdaBoost Classifier had the highest recall scores with the recall high/low risk being 0.91/0.94, making it the final best machine learning model to choose for further credit card analysis. 
