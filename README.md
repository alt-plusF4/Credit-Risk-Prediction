# Credit-Risk-Prediction
This project is about building a credit risk prediction model using the German Credit dataset. The project starts with data preprocessing, including data cleaning, feature engineering, and encoding categorical variables. XGBoost is used for predictive modelling.

Data Set Information:

![image](https://user-images.githubusercontent.com/58546519/233623449-d52f81d5-0474-4c75-8a1b-69c32678c8a3.png)


Two datasets are provided. the original dataset, in the form provided by Prof. Hofmann, contains categorical/symbolic attributes and is in the file "german.data".


For algorithms that need numerical attributes, Strathclyde University produced the file "german.data-numeric". This file has been edited and several indicator variables added to make it suitable for algorithms which cannot cope with categorical variables. Several attributes that are ordered categorical (such as attribute 17) have been coded as integer. This was the form used by StatLog.


This dataset requires use of a cost matrix (see below)

..... 1 2
----------------------------
1 0 1
-----------------------
2 5 0

(1 = Good, 2 = Bad)


The rows represent the actual classification and the columns the predicted classification.


It is worse to class a customer as good when they are bad (5), than it is to class a customer as bad when they are good (1).


Source - https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29
