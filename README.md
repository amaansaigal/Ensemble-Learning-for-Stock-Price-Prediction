## Ensemble Learning for Stock Price Prediction
### Introduction
This repository is dedicated to predicting the stock prices of Tesla (TSLA) using ensemble learning methods, namely Bagging and AdaBoost. The goal is to utilize historical stock data to forecast future prices and evaluate the predictive power of these models.

#### Project Structure
data/: This folder contains the dataset used for the analysis, sourced from Yahoo Finance.
notebooks/: Jupyter Notebooks with step-by-step analysis and code.
src/: Source code for custom Python functions used within the Notebooks.
output/: Output graphs and model performance metrics.
requirements.txt: Required Python packages for replication.
Data
The data spans from January 1, 2018, to January 1, 2023, including daily stock prices of TSLA. The key feature used for prediction is the Adjusted Close price, with lagged values serving as predictors.

#### Methodology
Data was sourced using the yfinance library.
Lagged features were created to use past stock prices to predict future ones.
The dataset was split into training and test sets to evaluate model performance.
Bagging and AdaBoost regressors were trained on the dataset.
Model performance was evaluated using the Mean Squared Error (MSE) metric.
Predictions and residuals were visualized to understand model accuracy.


#### Analysis
The analysis is divided into multiple Jupyter Notebooks:

data_collection.ipynb: Fetching and initial exploration of the stock price data.
data_preparation.ipynb: Data cleaning, feature engineering, and preparation.
model_training.ipynb: Training of the Bagging and AdaBoost ensemble models.
model_evaluation.ipynb: Evaluation of the models, including MSE calculation.
visualizations.ipynb: Graphical representation of the models' predictions vs. actual prices, and the analysis of residuals.
Results
The AdaBoost model exhibited a lower MSE compared to the Bagging model, indicating a better fit to the data.
Residual plots revealed the presence of patterns in prediction errors, suggesting areas for model improvement.
The analysis demonstrated that while ensemble methods can predict stock price movements to a certain degree, they also have limitations, especially when dealing with volatile markets.
