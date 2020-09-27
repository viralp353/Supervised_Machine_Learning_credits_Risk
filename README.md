# Supervised_Machine_Learning_credits_Risk


## Background:


Credit risk is an inherently unbalanced classification problem, as the number of good loans easily outnumber the number of risky loans. Therefore, We’ll need to employ different techniques to train and evaluate models with unbalanced classes. To use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.final task is to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.


## Objectives:


The goals of this challenge :

*  Implement machine learning models.


*  Use resampling to attempt to address class imbalance.


*  Evaluate the performance of machine learning models.


*  Train a logistic regression classifier (from Scikit-learn) using the resampled data.


*  Calculate the balanced accuracy score using balanced_accuracy_score from sklearn.metrics.


*  Generate a confusion_matrix.


* Print the classification report (classification_report_imbalanced from imblearn.metrics).




## Resources:

*  imbalanced-library

*  jupyter notebook

*  csv

*  Supervised Machine learning



## Challenge_Summary:

#### (1)Credit Risk Resampling Techniques:


In this section, I compared oversampling,Undersampling &Combine algorithms to determine which algorithm results in the best performance.I did oversample the data using the naive random oversampling algorithm and the SMOTE algorithm.and I used undersampling the data using Cluster Centroids algorithm and Combination  data using the SMOTEENN algorithm For each algorithm.


#####  Naive Random Oversampling:


For Analysis, I used oversample the data using the naive random oversampling algorithm.I got count of the target classes like (low_risk: 51352) & (high_risk: 260 ).Then I used the resampled data to train a logistic regression model.I got  0.66 balanced accuracy score. Based on confusion matrix,I got (TRUE POSITIVE:57),(FALSE NEGATIVE:30),(FALSE POSITIVE:5694),(TRUE NEGATIVE:11424).For imbalanced_classification_report, We see that on table.


![Naive Random Oversampling](https://user-images.githubusercontent.com/65969608/94352869-f5121d00-002f-11eb-93e9-cea69ac2956d.png)






##### SMOTE Oversampling:


For Analysis, I used oversample the data using the SMOTE Oversampling algorithm.I got count of the target classes like (low_risk: 51352) & (high_risk: 260 ).Then I used the resampled data to train a logistic regression model.I got  0.63 balanced accuracy score. Based on confusion matrix,I got (TRUE POSITIVE:54),(FALSE NEGATIVE:33),(FALSE POSITIVE:6163),(TRUE NEGATIVE:10955).For imbalanced_classification_report, We see that on table.






![SMOTE Oversampling](https://user-images.githubusercontent.com/65969608/94352872-0eb36480-0030-11eb-9394-0ce1dba4388b.png)


##### Undersampling:

For Analysis, I used undersample the data using the Cluster Centroids algorithm .I got count of the target classes like (low_risk: 260) & (high_risk: 260 ).Then I used the resampled data to train a logistic regression model.I got  0.52 balanced accuracy score. Based on confusion matrix,I got (TRUE POSITIVE:56),(FALSE NEGATIVE:31),(FALSE POSITIVE:10221),(TRUE NEGATIVE:6897).For imbalanced_classification_report, We see that on table.


![cluster](https://user-images.githubusercontent.com/65969608/94352900-779adc80-0030-11eb-9e3c-970018b3659a.png)


##### Combination (Over and Under) Sampling:


For Analysis, I used resample the data using the SMOTEENN algorithm .I got count of the target classes like (low_risk: 68460) & (high_risk: 62011 ).Then I used the resampled data to train a logistic regression model.I got  0.63 balanced accuracy score. Based on confusion matrix,I got (TRUE POSITIVE:61),(FALSE NEGATIVE:26),(FALSE POSITIVE:7294),(TRUE NEGATIVE:9824).For imbalanced_classification_report, We see that on table.




![combine](https://user-images.githubusercontent.com/65969608/94352885-43bfb700-0030-11eb-93e1-8d55f4c6db2c.png)


#### (2)Extension:



##### Balanced Random Forest Classifier:


![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/65969608/94352800-2a6a3b00-002f-11eb-84c9-ae67cda330c2.png)





##### Easy Ensemble AdaBoost Classifier:

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/65969608/94352838-92208600-002f-11eb-9dfb-de689f8041d9.png)


