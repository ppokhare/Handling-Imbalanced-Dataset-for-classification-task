# Handling-Imbalanced-Dataset-for-classification-task

In real life, almost all the data that you gathered will be highly imbalanced. For example, if you are a credit card company, then you will see a lot less non-fraudulent transactions in comparison to a fraudulent transaction. If you are a credit approval agency, then you will see a lot less default class in comparison to a non-default class. If you are a telecom company and trying to predict if your customers are likely to cancel their subscription, then you will find imbalances in your dataset as well.

There are various tactics to tackle this problem of imbalanced data set, but in this project, I am using two ways: Use of robust evaluation metrics (F1 score) and to oversample the least occurring class to avoid overfitting during the training process. 

 I trained Logistic Regression, SVMs, K-Nearest Neighbor, Decision Trees, Random Forests, and AdaBoost in higly imbalanced occupancy datasets from UCI Machine Learning Repository[1] and evaluated their training/testing F1 score. Extensive hyperparameter tunning and 5-fold cross-validation is used with 20:80 and 80:20 train test split. Testing F-1 score of 98.24%. 


[1] https://archive.ics.uci.edu/ml/datasets.php
