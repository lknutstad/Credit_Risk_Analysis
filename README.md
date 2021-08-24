# Credit Risk Analysis

## Overview

### Purpose

LendingClub, a peer-to-peer lending services company, wants to predict credit risk with machine learning.  Jill requests help using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling to best predict credit risk.

## Results

### Random Oversampler

The Random Oversampler model was accurate 64 % of the time (accuracy score = 0.64) 

- The precision of the high-risk loan prediction is almost 0, indicating very poor predictive power.
- The recall for high-risk loans is 0.69, indicating a significant number of false negatives
- The F1 score is extremely low for high-risk loans at 0.02
- Overall, the RandomOversampler model is a poor predictor of high risk loans.


### SMOTE Oversampling

The SMOTE oversampling model was accurate 66.2 % of the time (accuracy score = 0.662) 

- The precision of the high-risk loan prediction is almost 0, indicating very poor predictive power.
- The recall for high-risk loans is 0.63, indicating a significant number of false negatives
- The F1 score is extremely low for high-risk loans at 0.02
- Overall, the SMOTE oversampling model is a poor predictor of high risk loans.

### Cluster Centroid Undersampling

The Cluster Centroid Undersampling model was accurate 55.4 % of the time (accuracy score = 0.554) 

- The precision of the high-risk loan prediction is almost 0, indicating very poor predictive power.
- The recall for high-risk loans is 0.69, indicating a significant number of false negatives
- The F1 score is extremely low for high-risk loans at 0.01
- Overall, the Cluster Centroid Undersampling model is a poor predictor of high risk loans.

### Combination (Under/Over) Sampling

The Combination Sampling model was accurate 64.4 % of the time (accuracy score = 0.644) 

- The precision of the high-risk loan prediction is almost 0, indicating very poor predictive power.
- The recall for high-risk loans is 0.72, indicating a significant number of false negatives
- The F1 score is extremely low for high-risk loans at 0.02
- Overall, the Combination Sampling model is a poor predictor of high risk loans.

### Balanced Random Forest Classifier

The Balanced Random Forest Classifier model was accurate 78.8 % of the time (accuracy score = 0.788) 

- The precision of the high-risk loan prediction is 0.03, indicating a large number of false postives.
- The recall for high-risk loans is 0.70, indicating a significant number of false negatives
- The F1 score is low for high-risk loans at 0.06
- Overall, the Combination Sampling model is a moderate predictor of high risk loans.

### Easy Ensemble AdaBoost Classifier

The Easy Ensemble AdaBoost Classifier model was accurate 93.1 % of the time (accuracy score = 0.931) 

- The precision of the high-risk loan prediction is 0.09, indicating a large number of false postives.
- The recall for high-risk loans is 0.92, indicating a significant number of false negatives
- The F1 score is low for high-risk loans at 0.16
- Overall, the Easy Ensemble AdaBoost Classifier model is a predictor of high risk loans

## Summary

Our reccomendation to LendingClub is to implement the Easy Ensemble AdaBoost model to analyze high risk credit profiles as this model was most accurate.
