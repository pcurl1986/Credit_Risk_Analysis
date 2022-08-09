# Credit_Risk_Analysis
## Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were used to train and evaluate models with unbalanced classes. Various libraries and algorithms were used to build and evaluate models using resampling including:

* imbalanced-learn
* scikit=learn
* RandomOverSampler
* SMOTE algorithms
* ClusterCentroids algorithm
* SMOTEENN algotithm
* BalancedRandomForestClassifier (bias reduction model)
* EasyEnsembleClassifier (bias reduction model)

## Purpose
* Explain how a machine learning algorithm is used in data analytics.
* Create training and test groups from a given data set.
* Implement the logistic regression, decision tree, randomon forest, and support vector machine algorithms.
* Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
* Compare the advantages and disadvantages of each supervised learning algorithm.
* Determine which supervised learning algorithm is best used for a given data set or scenario.
* Use ensemble and resampling techniques to improve model performance.

Results:
Here are the results for the six machine learning modules.

### Naive Random Oversampling

![image](https://user-images.githubusercontent.com/101307058/183572481-3fbad0e3-367a-40f3-b133-0a9ddfd20de3.png)

* Balanced Accuracy:0.6293939430565123
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall High/Low risk = .57/.68

### Smote Oversampling

![image](https://user-images.githubusercontent.com/101307058/183572683-05618525-a453-45c8-86d6-56ed1660b75e.png)

* Balanced Accuracy:0.6277008271188627
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall High/Low risk = .62/.63

### Undersampling

![image](https://user-images.githubusercontent.com/101307058/183572823-55ffe438-7dc6-4d72-8ae3-b0567091b134.png)

* Balanced Accuracy:0.6277008271188627
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low = .61/.45

### Combination Under-Over Sampling

![image](https://user-images.githubusercontent.com/101307058/183572941-0e8e7b40-b5f2-4920-af6f-7bd04928467c.png)

* Balanced Accuracy:0.5295655712277054
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low = .70/.58

### Balanced Random Forest Classifier

![image](https://user-images.githubusercontent.com/101307058/183573034-9fa89073-67c8-4061-a23d-e8b0d50870e4.png)

* Balanced Accuracy:0.7885466545953005
* Precision: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall: High/Low = .70/.87

### Easy Ensemble AdaBoost Classifier

![image](https://user-images.githubusercontent.com/101307058/183573130-a4397a32-5923-4603-bfa3-68d787be35e7.png)

* Balanaced Accuracy:0.9316600714093861
* Precision: The precision is low for High-risk and is high for Low-risk loans.
* Recall: High/Low risk = .92/.94

### Summary:

When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy. The other models were below .80 balanced accuracy. The precision for all models were similar and within an appropriate range. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the best machine learning model to choose for further credit card analysis.
