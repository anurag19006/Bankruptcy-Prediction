# Bankruptcy-Prediction

The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined on the business regulations of the Taiwan Stock Exchange. The target variable has binary values making this a classification problem

## Dataset

It’s a highly unbalanced dataset, one class is in significantly large portion than the other.
It has around 7000 rows with 96 predictors.

## EDA and Preprocessing

*There are no missing values in the entire dataset.
*All the columns  are numerical and scaled.
*To balance the dataset we have used various data balancing techniques.
*To deal with high dimensionality we have used PCA which reduced column count 96 to 11-14 while capturing 0.99 information.
*Data splitted into 70:30 ratio for training and validation set.

## Predictive Modeling 

We trained below models on Original Data, Undersampled Data, Oversampled Data, SMOTE sampled data and PCA dimension reduced data.
-Logistic Regression 
-Naive Bayes
-Random forest 
-Neural Network

