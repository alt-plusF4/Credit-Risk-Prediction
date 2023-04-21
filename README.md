# Credit-Risk-Prediction
This project is about building a credit risk prediction model using the German Credit dataset. The project starts with data preprocessing, including data cleaning, feature engineering, and encoding categorical variables. XGBoost is used for predictive modelling.

Data Set Information:

[{"index":0,"status":1,"duration":6,"credit_history":5,"purpose":4,"credit_amount":1169,"savings_account":5,"employment_duration":5,"installment_rate":4,"status_sex":3,"other_debtors":1,"present_residence":4,"property":1,"age":67,"other_installment_plans":3,"housing":2,"number_credits":2,"job":3,"people_liable":1,"telephone":1,"foreign_worker":0},{"index":1,"status":2,"duration":48,"credit_history":3,"purpose":4,"credit_amount":5951,"savings_account":1,"employment_duration":3,"installment_rate":2,"status_sex":2,"other_debtors":1,"present_residence":2,"property":1,"age":22,"other_installment_plans":3,"housing":2,"number_credits":1,"job":3,"people_liable":1,"telephone":0,"foreign_worker":0},{"index":2,"status":4,"duration":12,"credit_history":5,"purpose":7,"credit_amount":2096,"savings_account":1,"employment_duration":4,"installment_rate":2,"status_sex":3,"other_debtors":1,"present_residence":3,"property":1,"age":49,"other_installment_plans":3,"housing":2,"number_credits":1,"job":2,"people_liable":2,"telephone":0,"foreign_worker":0},{"index":3,"status":1,"duration":42,"credit_history":3,"purpose":3,"credit_amount":7882,"savings_account":1,"employment_duration":4,"installment_rate":2,"status_sex":3,"other_debtors":3,"present_residence":4,"property":2,"age":45,"other_installment_plans":3,"housing":3,"number_credits":1,"job":3,"people_liable":2,"telephone":0,"foreign_worker":0},{"index":4,"status":1,"duration":24,"credit_history":4,"purpose":1,"credit_amount":4870,"savings_account":1,"employment_duration":3,"installment_rate":3,"status_sex":3,"other_debtors":1,"present_residence":4,"property":4,"age":53,"other_installment_plans":3,"housing":3,"number_credits":2,"job":3,"people_liable":2,"telephone":0,"foreign_worker":0}]


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
