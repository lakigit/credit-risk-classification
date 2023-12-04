# Module 20 Challenge : Supervised Learning

# Background

The objective of this project is to train and evaluate a model that can accurately assess loan risk using various techniques. The dataset used for analysis comprises of previous lending activities from a peer-to-peer lending services company. The goal is to create a model that can determine the creditworthiness of borrowers with precision. 

Upon importing a CSV file, the data should be separated into labels and features. The `loan_status` column should be used as the label (y), while the remaining columns should be used as features (X). A value of 0 in the `loan_status` column indicates that the loan is healthy, while a value of 1 indicates that the loan has a high risk of defaulting. The next step is to split the data into training and testing using the `train_test_split` function.

In order to create a regression model, it is recommended to employ the logistic regression model when dealing with binary data. The process of fitting the regression model involves assigning the model and subsequently utilizing the training data. Once the model has been trained, predictions can be made using the testing data. Finally, it is necessary to create a confusion matrix and classification report. To accomplish this, it is essential to import the relevant dependencies, namely `confusion_matrix` and `classification_report` respectively. 


# Results

# Confusion matrix

array([[18663,   102],
       [   56,   563]], dtype=int64)

# Classification Report

 precision    recall  f1-score   support

  Healthy Loan       1.00      0.99      1.00     18765
High-Risk Loan       0.85      0.91      0.88       619

      accuracy                           0.99     19384
     macro avg       0.92      0.95      0.94     19384
  weighted avg       0.99      0.99      0.99     19384
