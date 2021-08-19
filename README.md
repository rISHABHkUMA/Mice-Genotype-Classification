# Mice-Genotype-Prediction
##  Project Description
This project is for predicting "Genotype" of mice based on expression level of 77 different proteins. It is a binary classification problem. Three different types of ML 
algorthms viz. logistic regression with L1 regularizaiton, support vector machines and random forest classification are used. Data exploration, visualization and preprocessing 
were done prior to use classification algorithms. Implementation of all ML algorithms, data preprocessing and hyperparameters selection were done using inbuilt function from 
scikit learn library in python. All code is present in a single jupyter notebook "code.ipynb" file and was run on google colab server.

## Data
Data is taken from Mice Protein Expression Data Set at UCI ML repo https://archive.ics.uci.edu/ml/machine-learning-databases/00342/Data_Cortex_Nuclear.xls
The downloaded file is present in Data folder. For more information on data please visit https://archive.ics.uci.edu/ml/datasets/Mice+Protein+Expression

## Exploratory Data Analysis 
1. It was found that there are certain values missing in the given data. **Multivariate Feature Imputation** is used to estimate these missing values.
2. High correlation between some features were found. Only one of the highly correlated features was kept and others were dropped(**Feature Reduction**)

## Preprocessing
1.**Features were normalized** prior to prediction using standard scaler from sklearn preprocessing module.

## Hyperparameter selection
**Grid search** over range of hyperparameters was done and best parameters was selected using **k-fold cross validation** on training data.

## Algorithms used
1. Logistic regression with L1 regularization.
2. Support vector classification.
3. Random forest classification.


## Note: 
If you are trying to run the code in your system then make sure all required libraries and data files are present. ALternatively the notebook code.ipynb can be directly
uploaded and run on google colab server without any additional installation.
