# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to predict credit risk using a variety of techniques to train machine learning models.

## Results
#### Naive Random Oversampling
  - Balanced Accuracy Scores
    - The oversampling method returns an accuracy score of 0.644.
  - Precision
    - The precision for high risk loans is only 0.01 which is a poor result from using Oversampling. This means the model is predicting more high risk loans then there are in reality.
  - Recall
    - The model returns a recall score of 0.64. This means the model is accounting for over half of the loans that are actually high risk.

#### SMOTE Oversampling
  - Balanced Accuracy Scores
    - The oversampling method returns an accuracy score of 0.6167.
  - Precision
    - The precision for high risk loans is only 0.01 which is a poor result. This means the model is predicting more high risk loans then there are in reality.
  - Recall
    - The model returns a recall score of 0.57. This means the model is accounting for slightly over half of the loans that are actually high risk.

#### Undersampling
  - Balanced Accuracy Scores
    - The oversampling method returns an accuracy score of 0.649.
  - Precision
    - The precision for high risk loans is only 0.01 which is a poor result. This means the model is predicting more high risk loans then there are in reality.
  - Recall
    - The model returns a recall score of 0.74. This model does a better job at catching all high risk loans.

#### Combination Over and Under Sampling
  - Balanced Accuracy Scores
    - The oversampling method returns an accuracy score of 0.66.
  - Precision
    - The precision for high risk loans is only 0.01 which is a poor result. This means the model is predicting more high risk loans then there are in reality.
  - Recall
    - The model returns a recall score of 0.75. This model also is comparatively better for catching all high risk loans.

#### Balanced Random Forest Classifier
  - Balanced Accuracy Scores
    - The oversampling method returns an accuracy score of 0.80.
  - Precision
    - The precision for high risk loans is only 0.04 which is a poor result. This means the model is predicting more high risk loans then there are in reality.
  - Recall
    - The model returns a recall score of 0.70. This model also is comparatively better for catching all high risk loans.

#### Easy Ensemble AdaBoost
  - Balanced Accuracy Scores
    - The oversampling method returns an accuracy score of 0.70.
  - Precision
    - The precision for high risk loans is 0.77. This model does a comparetively better job at limiting False Positives.
  - Recall
    - The model returns a recall score of 0.41. This model does not do a good job of accounting for high risk loans.

## Summary
Each of the models have large weaknesses when predicting whether a loan is high risk or not. While most of the models have low precision scores, predicting false positives at a higher rate is not as detrimental as there is a higher chance of catching a greater percentage of high risk loans. 

The model I recommend is the Combination Over and Under Sampling. While this model has a lower accuracy score at 0.66 than other models, it does a better job at limiting false negatives. This is extremely important as the goal of this model is to predict for high risk loans. Limiting the number of false negatives reduces the number of high risk loans that go undetected. It would be important to continually refine this model before heavily relying on it as there is still a significant number of high risk loans that go undetected. 
