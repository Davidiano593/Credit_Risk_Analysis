# Credit Risk Analysis

## Overview

The purpose of this project is to use machine learning to predict and make decisions on a specific topic. Machine Learning is a discipline in the field of Artificial Intelligence that, through algorithms, gives computers the ability to identify patterns in massive data and make predictions (predictive analysis). This learning allows computers to perform specific tasks autonomously, that is, without the need to be programmed.
In this project we will look at credit risk as it is an inherently unbalanced rating problem, as good loans easily outnumber risky loans. Therefore, we must use different techniques to train and test unbalanced models.

## Summary

After analyzing the loan applications from our database, we classify the applications as "low risk" and "high risk" where the applications with "loan status" are classified as low risk and the others as high risk.

![This is an image](https://i.pinimg.com/originals/a9/6e/07/a96e07c02ccb1176d27f7ae789d2aefd.png)

When applying the training and testing, it gave us as a result that 51366 are within "low risk" and 246 as "high risk" in the training and in the test: "low risk": 17104 and "high risk": 101

## Using Resample Models to predict Credit Risk

Using the oversampler model we were able to match the results of both classifications.

![This is an image](https://i.pinimg.com/originals/a5/72/ec/a572ec07ad76caaece4df40534775bbd.png)

- We obtained a precision of 65%

![This is an image](https://i.pinimg.com/originals/cb/e4/04/cbe404525ee7635e181971e0f6324578.png)

- The recall of "high risk" is 73% with a 1% precission
- The recall of "low risk" is 58% with a 100% precission.

## Smote

Using the SMOTE model we were able to increase the size of the smallest value, creating new values that approximate the closest values of the smallest class.

- The accuracy score is: 66.2%

![This is an image](https://i.pinimg.com/originals/d9/bc/ec/d9bcec01463048c01446c7c702576200.png)

- The recall of "high risk" is 63% with a 1% precission
- The recall of "low risk" is 69% with a 100% precission.

## Undersampling

Using the ClusterCentroids model we were able to classify 246 records as "high risk" and 246 as "low risk".


- We obtained a precision of 54.4%

![This is an image](https://i.pinimg.com/originals/39/eb/42/39eb4271f61df9a04de13b6098ebb90f.png)

- The recall of "high risk" is 69% with a 1% precission
- The recall of "low risk" is 40% with a 100% precission.


## Ensemble Classifier for credit Risk

Comparing the two models, joining the Ensemble classifier, this model classifies 51366 as "high risk" and 246 as "low risk"

![This is an image](https://i.pinimg.com/originals/be/01/f9/be01f9cb17070cf27b8f69ceb52282aa.png)

## Balanced Random Forest Classifier

A balanced random forest randomly under-samples each boostrap sample to balance it.

- The accuracy score is 78.8% which increased about 24%

![This is an image](https://i.pinimg.com/originals/7a/9b/78/7a9b78ca784aa98ed600a170fb15759c.png)

- The recall of "high risk" is 70% with a 3% precission
- The recall of "low risk" is 87% with a 100% precission.

## Easy Ensemble AdaBoost Classifier

EasyEnsemble Classifier Model, combina decisiones individuales para clasificar nuevos ejemplos

- The accuracy score is 93.1%

![This is an image](https://i.pinimg.com/originals/0e/4a/b2/0e4ab2baf098c7ee993988818046106e.png)

- The recall of "high risk" is 92% with a 9% precission
- The recall of "low risk" is 94% with a 100% precission.

## Conclussion
By comparing both models, I can conclude that the Ensemble Classifier model gave us better values, the EasyEnsembleClassifer gave us an accuracy of 93.1% and it was also the best prediction for "high risk" loan applicants:
- The recall of "high risk" is 92% with a 9% precision
- The recall of "low risk" is 94% with a 100% precision.
After analyzing the data and comparing the final results, we can observe the difference between the data obtained at the beginning, where 1% of the applicants were classified as "high risk" and 99% were "low risk", the data was completely biased and we had to match the results more using various machine learning tools that gives us a more real and easier result when making a decision.