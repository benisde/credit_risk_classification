# Overview of the Analysis

Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. Using a dataset of historical lending activity from a peer-to-peer lending services company, purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.

In this analysis, used various techniques to train and evaluate models with imbalanced classes.

This analysis is performed on the original dataset using variables like value_counts and then resampled the dataset for accuracte prediction of the model.

Using the imbalanced-learn library, defined a logistic regression model to compare two versions of the dataset. First, using the original dataset. Second, resampled the data by using the RandomOverSampler module from the imbalanced-learn library.

In this analysis LogisticRegression classifier and the resampled data is used to fit the model and make predictions. The RandomOverSampler module from the imbalanced-learn library is used to resample the data.

For both cases, analyzed the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.


## Results

* Machine Learning Model 1:
  *  Logistic Regression Model with the Original Data
        * Accuracy: 95.20%  
        * Precision: 85% 
        * Recall: 91%
<br></br>
* Machine Learning Model 2:
  * Logistic Regression Model with Resampled Training Data
        * Accuracy: 99%  
        * Precision: 84% 
        * Recall: 99%

## Summary

Resampling the lending data performing the Logistic Regression model provided better accuracy compared to the original version of the data-set. This is because of higher recall score and accuracy score for the resampled training data.
Predicting High-risk loan ("1") is more important compared to Healthy Loan ("0").
The recall score High-risk loans using Logistic Regression model on the original data is 91% where as its 99% using resampled data. The accuracy score High-risk loans using Logistic Regression model on the original data is 95% where as its 99% using resampled data. Hence, Logistic Regression Model with Resampled Training Data has better performance to identify the credit worthiness of boorrowers.
