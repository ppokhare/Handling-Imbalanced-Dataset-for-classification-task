# FRAUDULENT CREDIT CARD TRANSACTION PREDICTION

In real life, almost all the data that you gathered will be highly imbalanced. For example, if you are a credit card company, then you will see a lot fewer non-fraudulent transactions in comparison to a fraudulent transaction. If you are a credit approval agency, then you will see a lot less default class in comparison to a non-default class. If you are a telecom company and trying to predict if your customers are likely to cancel their subscription, then you will find imbalances in your dataset as well.

There are various tactics to tackle this problem of an imbalanced data set:

**Dataset level solutions:** Get more data; Use sampling techniques such as random oversampling, random undersampling, KNN based random oversampling(STOME)

**Objective/ Loss Function level solution:** use appropriate weights on the positive and negative class; custom loss function(Focal Loss)  
![alt text](https://github.com/ppokhare/Handling-Imbalanced-Dataset-for-classification-task//blob/master/focal_loss.png?raw=true "Focal Loss")

**Evaluation metrics level solutions:** Accuracy is useless as your data is more imbalanced. $F_\beta$ and AUC-PR are better evaluation metrics. Depending on what's more important precision or recall, $\beta$ can be adjusted. 


**Result Summary:**
|      Classifier     | Training F1 SCore | Testing F1 Score |
|:-------------------:|:-----------------:|:----------------:|
| Logistic Regression |      0.715426     |     0.735632     |
|    Decision Tree    |      0.865526     |     0.838710     |
|    Random Forest    |      0.896894     |      0.80898     |
|       Xgboost       |      0.995506     |     0.884211     |
|   Neural Networks   |      0.886457     |     0.853932     |


**Resources:**  
Xgboost Hyperparameters: https://xgboost.readthedocs.io/en/latest/parameter.html#parameters-for-tree-booster  
Original Focal Loss paper: https://arxiv.org/abs/1708.02002    
Focal Loss explanation blog: https://leimao.github.io/blog/Focal-Loss-Explained/    
Handling imbalanced data problem guide: https://www.analyticsvidhya.com/blog/2017/03/imbalanced-data-classification/  
Dataset: https://www.kaggle.com/mlg-ulb/creditcardfraud  
