# Credit_Risk_Analysis

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Client asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

We used different types of sampling for this exercise: Naive Random oversampling, SMOTE oversampling, Undersampling (Cluster Centroids), Combination (over and under) Sampling aka SMOTEENN, Ensemble Leaners/Random Forest Classifier and the Adaptive Boosting Ensemble AdaBosst Classifier. Each one of the different methodologies have specific strengths and weakness yet the one that performed the best was Adaboost Classifier with Balanced Accuracy Score of 92.54%; the confusion matrices was also the most accurate, with the highest number of true positives and true negatives; lastly the Imbalance Classification report was miles ahead of the rest of the models. 

## Summary

Since we are using these models for loan approvals, sensitivity is more important than precision. That is, it is more important to make sure banks protect themselves (and their potential customers) by not approving loans that will fail. The Adaptive Boosting Classifier model will protect a bank’s brand/reputation. Also, we aren't so concern about precision because, the bank has loan officer(s) that can review and approve a loan whose feature's value(s) have been deemed as high-risk. Using the Adaptive Boosting Classifier model is well suited for determining whether a loan is high risk or not.
