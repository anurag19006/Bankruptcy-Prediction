# Bankruptcy-Prediction

The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined on the business regulations of the Taiwan Stock Exchange. The target variable has binary values making this a classification problem

## Dataset

It’s a highly unbalanced dataset, one class is in significantly large portion than the other.
It has around 7000 rows with 96 predictors.

![image](https://user-images.githubusercontent.com/57527313/218591788-48918f0a-66e3-4fb6-8365-95c78d8a9e7b.png)

## EDA and Preprocessing

* There are no missing values in the entire dataset.
* All the columns  are numerical and scaled.
* To balance the dataset we have used various data balancing techniques.
* To deal with high dimensionality we have used PCA which reduced column count 96 to 11-14 while capturing 0.99 information.
* Data splitted into 70:30 ratio for training and validation set.

## Data Balancing

![image](https://user-images.githubusercontent.com/57527313/218591956-5de2618b-9185-4064-94b5-eb9d40116c77.png)

## Predictive Modeling 

We trained below models on Original Data, Undersampled Data, Oversampled Data, SMOTE sampled data and PCA dimension reduced data.
- Logistic Regression 
- Naive Bayes
- Random forest 
- Neural Network

## Performance Analysis

- We have used class weights while training the model on original unbalanced data.
- Along with basic models we also trained a Neural Network with different architectures for original and PCA reduced dataset.
- Random forest turned out to be the best performing model on Undersampled Data.

## Use Cases

- In medical domain and financial domain many of the data analysis tasks suffers from unbalanced data anomaly. 
- This problem provides us the opportunity to work with unbalanced dataset.
- The results will help the organizations keep track of the accurate predictors that actually cause decline of the organization. This in turn will help them carry our - specific operations to save the bank from bankruptcy.

## Recommendation

- Objectives we met / Learnings
  - Various techniques to deal with highly unbalanced dataset
  - PCA with high dimensional data
  - Trained multiple models with different hyper parameters
- Future Work
  - To study and try more complex Neural Network models.

## References

- Data set : https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction
- https://towardsdatascience.com/how-to-balance-a-dataset-in-python-36dff9d12704
- https://www.datacamp.com/tutorial/understanding-logistic-regression-python
- https://medium.com/luca-chuangs-bapm-notes/build-a-neural-network-in-python-binary-classification-49596d7dcabf
- https://datascienceparichay.com/article/get-correlation-between-columns-of-pandas-dataframe/
- https://stackoverflow.com/questions/4700614/how-to-put-the-legend-outside-the-plot
