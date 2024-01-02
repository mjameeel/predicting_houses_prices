# Prediction of Houses Prices in Mexico

![Houses for Sale](images/house.jpg)
Image by <a href="https://pixabay.com/users/pexels-2286921/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=1836070">Pexels</a> from <a href="https://pixabay.com//?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=1836070">Pixabay</a>

## Introduction

The project is an example of a regression problem in machine learning. In this project, a Gradient Boosting Regressor was deployed to build, and test a model to predict the prices of houses with several features as contained in the data sets.

## Dependencies

The following libraries were imported and used in the project;
* Pandas
* Numpy
* Sklearn GradientBoostingRegressor
* Sklearn OneHotEncoder

## Data Cleaning

The data was cleaned before deploying to train model by dropping columns with high null count, filling numerical columns with appropriate values (median or 0), and then filling the categorical features null values with 'NA'.

## EDA

The numerical features of the train data was explored by ploting a histogram. The distriburion of the houses' features was explored.

## Spliting of Data and Model Building

The train data was split into target vector and features matrix using the train_test_split with test size of 20%. A pipeline of OneHotEncoder, SimpleInputter and GradientBoostingRegressor was deployed to buld the model. The model was then deployed to predict prices using test data. On evaluation, the model has a mean absolute error of 17588.88. Recall that the mean prices of the houses was determined to be 177806.31.

Details of the project is available in the project jupyter file.