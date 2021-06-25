# Credit_Risk_Analysis

## Overview:

The purpose of this assignment is to run machine learning algorithms on credit risk data and compare the difference in the algorithms and sampling techniques used for each.

## Results:

### Oversampling:

### Naive Random Oversampling

The model produced a balanced accuracy score of 0.64.
It produced a precision of 0.01 for high risk loans and 1.00 precision for low risk. It had a recall of 0.73 for high risk loans and 0.55 for low risk.

![image](https://user-images.githubusercontent.com/78934120/123340423-2dd91700-d51a-11eb-99bb-ad01b57ecdaa.png)

### SMOTE Oversampling

The model produced a balanced accuracy score of 0.66.
It produced a precision of 0.01 for high risk loans and 1.00 for low risk loans. It had a recall of 0.63 for high risk loans and 0.69 for low risk loans. 

![image](https://user-images.githubusercontent.com/78934120/123340554-5cef8880-d51a-11eb-99dd-b49f1647ce81.png)

### Undersampling:

### Cluster Centroid method:

The model produced a balanced accuracy score of 0.54.
It produced a precision of 0.01 for high risk loans and 1.00 for low risk loans. It had a recall of 0.69 for high risk loans and 0.4 for low risk loans.

![image](https://user-images.githubusercontent.com/78934120/123340749-bb1c6b80-d51a-11eb-98f3-25b9ebf41b7d.png)

### Combination Sampling (Over and Under):

### SMOTEENN

The model produced a balanced accuracy score of 0.65.
It produced a precision of 0.01 for high risk loans and 1.00 for low risk loans. It had a recall of 0.73 for high risk loans and 0.57 for low risk loans.

![image](https://user-images.githubusercontent.com/78934120/123340923-10f11380-d51b-11eb-8c0b-d281923dda9e.png)

### Ensemble Methods:

### Balanced Random Forest

The model produced a balanced accuracy score of 0.73.
It produced a precision of 0.06 for high risk loans and 1.00 for low risk loans. It had a recall of 0.5 for high risk loans and 0.95 for low risk loans.

![image](https://user-images.githubusercontent.com/78934120/123341042-40078500-d51b-11eb-9e3d-b30442cc41b2.png)

### Easy Ensemble 

The model produced a balanced accuracy score of 0.92.
It produced a precision of 0.05 for high risk loans and 1.00 for low risk loans. It had a recall of 0.93 for high risk loans and 0.9 for low risk loans.

![image](https://user-images.githubusercontent.com/78934120/123341157-7d6c1280-d51b-11eb-8a3a-7174a45ced87.png)

## Summary:

The ensemble methods had better balanced accuracy than the sampling methods. However, with the low recall on high risk loans that the balanced random forest model
provided I would not recommend using it over the SMOTEENN. Every model had great preecision on low risk loans however the sampling models did not have a good recall on
the low risk loans. Overall the best model is the Easy Ensemble model as it scores highly on everything where it is finding a lot of the low and high risk loans while still
offering comparable quality. Its high recall rate on high risk loans would make it the most useful model since it would catch more of the risky loans and allow for further 
investigation to determine their viability by other means. 
