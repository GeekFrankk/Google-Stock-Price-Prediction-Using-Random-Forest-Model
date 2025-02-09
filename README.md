# Stock Price Prediction Using Machine Learning

## Introduction
The main goal of this project is to predict the closing price of Google (GoG) stock using machine learning techniques.

## Data Collection
The historical stock price datasets for GoG were collected from Kaggle.(2004-2024)

## Data Preprocessing
- Converted 'Date' column to datetime format.
- Filled missing values using forward fill.
- Created additional features like moving averages and returns.

## Feature Engineering
- Created 10-day and 50-day moving averages.
- Calculated daily returns.

## Model Training and Evaluation
- Used Random Forest Regressor for prediction.
- Achieved a Mean Absolute Error (MAE) of 0.127.

## Model Deployment
- Saved the trained model using `joblib`.
- Created an API using Flask for making predictions.

## Conclusion
This model effectively estimates the stock's closing price with a good degree of accuracy. Potential enhancements include fine-tuning hyperparameters and experimenting with different machine learning approaches for improved performance.

## How to Use
1. Clone the repository.
2. Install required packages using `pip install -r requirements.txt`.
3. Run the Flask API using `python app.py`.
4. Make POST requests to the API endpoint `/predict` with JSON input for predictions.

