# Car Demand Forecasting
## Problem Statement
ABC is a car rental company based out of Bangalore. It rents cars for both in and out stations at affordable prices. The users can rent different types of cars like Sedans, Hatchbacks, SUVs and MUVs, Minivans and so on.

In recent times, the demand for cars is on the rise. As a result, the company would like to tackle the problem of supply and demand. The ultimate goal of the company is to strike the balance between the supply and demand inorder to meet the user expectations. The company has collected the details of each rental. Based on the past data, the company would like to forecast the demand of car rentals on an hourly basis.

## Objective
The main objective of the problem is to develop the machine learning approach to forecast the demand of car rentals on an hourly basis.

## Dataset
Dataset consisting of 18000+ records and 3 features-
* Date - date of year
* Hour - hour in a day
* Demand - car demand in corresponding hour
**Note -** This data is from 2018-2021

## Approach
The data given had no features except date and hour. So, I had to generate extra features from the date column by feature engineering. Extracted month_name, day, year, day_type, week_of_year. 
Performed Exploratory Data Analysis on the dataset, both univariate and multivariate analyses. Checked for questions like-
* Demand on weekends vs weekday
* Demand each month yearwise
* Ride on each month and day
* Checked correlation between each variable

For categorical features I applied one hot encoder and as the features were on different scales, so performed feature scaling to covert them on a same scale.
Used Linear Regression and Random Forest models to predict target variable demand. Random Forest was better in predicting, tuned hyperparameter 'max_depth'. Used differnt evaluation metrics like - MAE, MSE, RMSE, R2 score.
