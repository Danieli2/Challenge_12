# Challenge_12
***
# Module 12 Report
***

**Overveiw of the analysis** 

The purpose of this analysis is to use historical lending data from peer-to-peer lending to build a model which will detect and identify the credit worthiness of barrowers. The data included a loan status colunm which determined weather a loan was a healthy loan (0) or a risky loan (1). Every loan was catagorized into 1 or 0 depending on the other factors in the data set. The Value counts for the loans were unequally distributed with more healthy loans (0) than risky loans(1). The healthy loans are 75,036 and the risky loans are 2,500 This shows that there are more healthy loans than risky loan in the data set. After spliting the data set into a binary descion rule of healthy loans and Risky loans I then proceded to split the data between a test set and a train set or x_train and x_test followed by y_train and y_test. This will allow me to follow up with a logistical regression and determine accuracy and recall of the results of the data. Following up with a logistical regression requires me to make a logistical regression model with a random state of 1. I then fit the model with the train set of both x-train and y_train. Once the modle is fitted I then use the predict function on the test sets to determine the efficacy of my model at identifying healthy and risky loans. After this setep I evaluate how my model performed with the test set. I create three things to determine the efficacy of my model to identify the differing loans . first I create an balanced accuracy score followed by a confusion matrix to determine the results of the test ran by my model. The last step is to create a classification report which displays the precision score and the recall score. In total I created two logistical regression models one usig the original data and the other using the resampeling data. The two main methodes I used were the resampling methode and the logistical regression method.
***
**Results**

Machine Learning model 1:
This machine learning model involves a logistical regression using the the training setwhich fits the model to the data. This is followed by testing the model on the test set of data which themn is used for prediction on the test set. 
Balanced Accuracy score: 0.95
percision: 
        Healthy loans :1.00
        Risky loans : 0.85
Recall: 
    healthy Loans: 0.99
    Risky loans:  0.91
Machine learning Model 2:
This machine learning model  invloves a logistical regression model with an added step of a resampling methode in the process to allow for the model to better learn the data set. 
Balanced Accuracy score: 0.99
precision:
     Healthy loans: 1.00 
     Risky Loans:0.84
Recall: 
     healthy loans:0.99
     Risky loans:0.99
***
**Summary**

Both Models performed well and can beused for prediction because of the high degree of accuracy demonastrated by both models. However if pressed to make a decision on which model performs better it would have to be model 2 because of the higher accuracy scores. meaning that the accuracy of model two is 99% while the accuracy of model one is 95%. following this it is also true the model two also has a higher recal score for risky loans which means a higher chance of idetifiying risky loans then the first model. This advatage of the second model comes from the extra layer of analysis which is the resampling method incorperated into the the second model. In this case I beleive it is more important to predict the 1 because these repersents a risky loans where as a 0 represents a healthy loans so if the model does not identify a healthy loan then no harm done but if a model fails to identify a risky loan that is a problem worse then not finging a healthy loan.  
     
     
     
     
