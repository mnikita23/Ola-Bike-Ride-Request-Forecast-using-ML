# Ola-Bike-Ride-Request-Forecast-using-ML

## Problem Statement
The objective of this project is to forecast the number of bike ride requests received by Ola on a given day based on various weather and calendar features. Accurate forecasts can help in better fleet management and operational planning.

## Tools and Libraries Used
Python (Pandas, NumPy, Matplotlib, Seaborn)

Scikit-learn (Linear Regression, Decision Tree, Random Forest)

Holidays (for identifying public holidays)

Jupyter Notebook

## Dataset Description

The dataset includes the following features:

date: Date of observation

temp: Temperature in Celsius

humidity: Relative humidity (%)

windspeed: Wind speed (km/h)

count: Number of ride requests (target variable)

Additional features were engineered, such as:

day, month, year: extracted from date

is_weekend: whether the date falls on a weekend

is_holiday: determined using the holidays library

## Approach

Data Preprocessing

Handled missing values

Converted date column to datetime format

Extracted time-based features

Identified holidays using the holidays package

Exploratory Data Analysis

Plotted boxplots to detect outliers in temp and windspeed

Visualized trends using time series and bar charts

Feature Engineering

Created additional columns like is_holiday and is_weekend

Modeling

Split data into training and test sets

## Applied models:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Evaluated using RMSE and R² score


## Results and Conclusion

Random Forest Regressor performed the best with the highest R² score and lowest RMSE.

Weather and calendar-based features (e.g., temp, holiday, is_weekend) significantly impacted ride request volume.

This model can help Ola optimize driver allocation and surge pricing strategies.

## Future Work

Include real-time traffic or weather API integration

Apply time-series specific models (ARIMA, Prophet)

Build a web dashboard for operational use
