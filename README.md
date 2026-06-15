# Melbourne Airbnb Price Prediction using Regression Models

This project explores a regression-based machine learning workflow for predicting nightly Airbnb listing prices in Melbourne using listing, host, location, room, and review-related features.

The project was completed as part of my Computational Machine Learning coursework and has been converted into a portfolio-friendly version. The original dataset used for the assignment is not included in this repository due to assessment data-use restrictions.

## Project Overview

The goal was to predict the nightly price of an Airbnb listing based on structured features such as room type, location, accommodation capacity, bedrooms, bathrooms, review information, and host/listing attributes.

This is a supervised machine learning regression problem because the target variable is numerical.

## Methods Used

The workflow included:

* data inspection and exploratory data analysis
* train-validation splitting
* preprocessing of numerical and categorical features
* standardisation of numerical variables
* one-hot encoding of categorical variables
* model comparison
* hyperparameter tuning
* model evaluation using RMSE, MAE, and R²
* discussion of real-world limitations and ethical considerations

Three regression models were compared:

* Linear Regression
* Ridge Regression
* Lasso Regression

## Key Findings

Exploratory analysis showed that property size and capacity-related variables were important indicators of price. Features such as bedrooms, accommodates, beds, bathrooms, and room type showed clear relationships with nightly price.

The target variable was right-skewed, meaning most listings were in the lower price range while a smaller number of listings had very high prices. This made the prediction task more difficult for linear models.

## Model Selection

Ridge Regression performed best overall after validation and hyperparameter tuning. A moderate regularisation value improved generalisation slightly compared with ordinary Linear Regression.

The final selected model was:

**Ridge Regression with alpha = 10**

The model was useful as a basic decision-support tool, but it was not suitable as a fully automated pricing system because it struggled with expensive or unusual listings.

## Skills Demonstrated

* Python
* pandas
* NumPy
* scikit-learn
* Linear Regression
* Ridge Regression
* Lasso Regression
* feature preprocessing
* one-hot encoding
* model evaluation
* hyperparameter tuning
* responsible AI discussion

## Data Availability

The processed assignment dataset is not included in this repository because it was provided only for assessment use. This repository is intended to document the machine learning workflow and project learning outcomes without redistributing restricted data.
