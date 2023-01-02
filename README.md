# Overview of the analysis:

## Background
Credit risk is an inherently unbalanced classification problem as good loans outnumber risky loans. Therefore, I’ll be employing different techniques to train and evaluate models with unbalanced classes. 

## Purpose
To apply machine learning to solve a real-world challenge: credit card risk. I’ll be using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTEalgorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENNalgorithm. 

Finally, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

# Results:
## 1) Using RandomOverSampler
## The balanced accuracy scores 0.6456130066757718
## The precision and recall scores for the high_risk category are 0.01, 0.61 whereas the precision and recall scores for the low_risk are 1.00, 0.68 


'''

'''


## 2) Using SMOTE Oversampling
## The balanced accuracy scores 0.6234433606890912
## The precision and recall scores for the high_risk category are 0.01, 0.61 whereas the precision and recall scores for the low_risk are 1.00, 0.64

'''

'''


## 3) Using ClusterCentroids Undersampling
## The balanced accuracy scores 0.5164869808348542
## The precision and recall scores for the high_risk category are 0.01, 0.60 whereas the precision and recall scores for the low_risk are 1.00, 0.44

'''


'''


## 4) Using Combination (Over and Under) Sampling SMOTEENN
## The balanced accuracy scores 0.590320332297924
## The precision and recall scores for the high_risk category are 0.01, 0.70 whereas the precision and recall scores for the low_risk are 1.00, 0.58

'''

'''


## 5) Using Balanced Random Forest Classifier
## The balanced accuracy scores 0.7877672625306695
## The precision and recall scores for the high_risk category are 0.04, 0.67 whereas the precision and recall scores for the low_risk are 1.00, 0.91

'''

'''


## 6) Using Easy Ensemble Classifier
## The balanced accuracy scores 0.925427358175101
## The precision and recall scores for the high_risk category are 0.07, 0.91 whereas the precision and recall scores for the low_risk are 1.00, 0.94

'''


'''



# Summary:
Precision and recall scores are commonly used in machine learning to evaluate the performance of a classifier. Precision measures the proportion of positive predictions that are usually correct while recall measures the proportion of actual positive cases that were accurately predicted.

There is no "one size fits all" and so we can't say that an exact precision or recall score is the best. It all depends on the goal of the analysis and the specific context of the case. For example in a medical scenario, a higher precision score is more important than a high recall score because we would want to minimize the number of false positive predictions. Whereas in detection of fradulent activity a higher recall score is more suited because its more important to maximize the number of fraudulent cases that are detected. 

For this credit risk analysis, I would highly recommend Using Easy Ensemble Classifier since it has the best precision and recall scores of all the 6 models. The precision and recall scores for the high_risk category are 0.07, 0.91 whereas the precision and recall scores for the low_risk are 1.00, 0.94. The balanced accuracy scores  of 0.925427358175101 are the highest too. Using this tool would be the best in this context. Since we want to maximize the detection of high-risk category. 




