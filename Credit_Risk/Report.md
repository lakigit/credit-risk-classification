# Module 20 Challenge : Supervised Learning

# Background

The objective of this project is to train and evaluate a model that can accurately assess loan risk using various techniques. The dataset used for analysis comprises of previous lending activities from a peer-to-peer lending services company. The goal is to create a model that can determine the creditworthiness of borrowers with precision. 

Upon importing a CSV file, the data should be separated into labels and features. The `loan_status` column should be used as the label (y), while the remaining columns should be used as features (X). A value of 0 in the `loan_status` column indicates that the loan is healthy, while a value of 1 indicates that the loan has a high risk of defaulting. The next step is to split the data into training and testing using the `train_test_split` function.

In order to create a regression model, it is recommended to employ the logistic regression model when dealing with binary data. The process of fitting the regression model involves assigning the model and subsequently utilizing the training data. Once the model has been trained, predictions can be made using the testing data. Finally, it is necessary to create a confusion matrix and classification report. To accomplish this, it is essential to import the relevant dependencies, namely `confusion_matrix` and `classification_report` respectively. 


# Results

* **Confusion matrix**

![image](https://github.com/lakigit/credit-risk-classification/assets/138610916/1babec63-7f6b-4c9b-883f-24c6e2bedba4)


* **Classification Report**

![image](https://github.com/lakigit/credit-risk-classification/assets/138610916/5cfc167b-b1d7-438d-b30a-c4c0673112fe)

Model 01 (Healthy Loan): \
          f1-score: Since this value is 1, it tells us that the model does a very good job
