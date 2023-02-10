# Credit_Card_Fraud_Detection
The data set contains transactions made by credit cards in September 2013 by European cardholders. It consists of transactions that occured in 2 days, where 492 of the transactions are fraud, out of 284 807 transactions.

- The data set contains only numerical input values which are the result of a PCA transformation. Unfortunately due to confidentiality issues, more background information about the data and the original features cannot be provided. 
-  Features V1, V2 up to V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.
- 'Time' contains the seconds elapsed between each transaction and the first transaction in the data set. 'Amount' is the transaction amount, 'Class' is the response variable and it takes values `1 in case of fraud` and `0 otherwise`.


# Solution Overview

In this notebook, we aimed to develop a machine learning model for detecting fraudulent credit card transactions. The problem of credit card fraud is becoming increasingly prevalent and it is important to have an accurate and reliable system for detecting fraud in real-time.

We evaluated several machine learning models including logistic regression, random forest, and xgb classifier. We found that the xgb classifier performed the best with an accuracy of 84.884 on the testing data.

The model was able to accurately detect fraud with a precision of 93% and a recall of 78%. These results indicate that our model is capable of detecting the majority of fraudulent transactions while minimizing the number of false positive alerts.

One limitation of our analysis is that the dataset only includes a small subset of all possible features that could be used to detect fraud. Furthermore, the oversampling technique used to balance the class distribution may have resulted in overfitting.

In conclusion, our xgb classifier provides a promising solution for detecting credit card fraud in real-time. However, the oversampling technique used to balance the class distribution may have resulted in overfitting. A more robust solution could be achieved by using both oversampling and undersampling techniques, which would better balance the class distribution while also reducing the risk of overfitting. Future work could include incorporating additional features and testing the model on a larger and more diverse dataset.  Additionally, further investigation into using a combination of oversampling and undersampling techniques could lead to even better results.
