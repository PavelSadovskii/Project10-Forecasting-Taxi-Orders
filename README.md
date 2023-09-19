# Taxi Order Forecasting

## Project Description

Clear Taxi, a company specializing in airport taxi services, has collected historical data on taxi orders. To attract more drivers during peak hours, the company needs to forecast the number of taxi orders for the next hour. In this project, we build a model to make such predictions.

## Project Goal

The goal of this project is to create a model capable of predicting the number of taxi orders for the next hour. The quality metric for the model is RMSE (Root Mean Square Error), and its value on the test dataset should not exceed 48.

## Tools and Libraries

The following tools and libraries were used for this project:

- Pandas
- NumPy
- StatsModels
- Matplotlib
- Scikit-Learn
- LightGBM
- CatBoost

## Project Steps

### Step 1: Data Preparation

- Import the required modules and libraries.
- Load the data and view basic information about it.
- Resample the data at one-hour intervals.

### Step 2: Data Analysis

- Analyze time series differences in the data.
- View the data with different resampling intervals.
- Analyze trends and seasonality in the data.
- Explore the moving standard deviation.

### Step 3: Model Training

- Create additional features such as day of the month, day of the week, month, moving average, and lags.
- Split the data into training and test sets.
- Train a LinearRegression model for forecasting.
- Train a CatBoostRegressor model with hyperparameter tuning.

### Step 4: Model Testing

- Test the CatBoostRegressor model on the test dataset and calculate RMSE.
- Compare the predicted data with the actual values.

## Findings

During the project implementation, the following outcomes were achieved:

- Data was prepared for model training.
- Trends and seasonality in the data were identified, providing insights into its structure.
- Additional features capturing temporal dependencies were created.
- The CatBoostRegressor model was trained and achieved good results with an RMSE of 41.249 on the test dataset, meeting the project's goal.

These findings can be utilized by Clear Taxi to optimize operations and attract more drivers during peak hours.
