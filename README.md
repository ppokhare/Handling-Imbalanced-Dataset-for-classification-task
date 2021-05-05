# Handling-Imbalanced-Dataset-for-classification-task

In real life, almost all the data that you gathered will be highly imbalanced. For example, if you are a credit card company, then you will see a lot less non-fraudulent transactions in comparison to a fraudulent transaction. If you are a credit approval agency, then you will see a lot less default class in comparison to a non-default class. If you are a telecom company and trying to predict if your customers are likely to cancel their subscription, then you will find imbalances in your dataset as well.

There are various tactics to tackle this problem of imbalanced data set, but in this project, I am using two ways: Use of robust evaluation metrics (AUC Precision-Recall Curve, F1-score) and to use custom loss function (Focal Loss).

I used Neural Networks in highly imbalanced credit card transactions dataset to predict the fradulant cases. The positive class (frauds) is only 0.172% of all transactions.   

Test data Result:  
	AUC-PR score: 80.84%  
	F-1 score: 82.11%   
	Precision: 84.78%  
	Recall: 79.49%  
	Accuracy: No one care :)  

Original Focal Loss paper: https://arxiv.org/abs/1708.02002  
Really good explainion blog: https://leimao.github.io/blog/Focal-Loss-Explained/  
Dataset: https://www.kaggle.com/mlg-ulb/creditcardfraud
