# Currency Impact on S&P 500 ETF Prediction
## By: Brigilda Lleshi, Mario Penagos, Yousef Sersy, and Megan Eunpu
 


## Project Overview

This project aims to analyze the impact of currency fluctuations on the S&P 500 ETF (SPY) and predict the future direction of SPY based on the exchange rates of EUR/USD and JPY/USD. The analysis involves historical data collection, data processing, model training, and prediction using machine learning techniques.

## Objectives

1. **Collect and preprocess historical financial data**:
    - S&P 500 ETF (SPY) prices
    - EUR/USD exchange rates
    - JPY/USD exchange rates
2. **Analyze the historical trends and percentage changes** of SPY, EUR/USD, and JPY/USD.
3. **Develop and train machine learning models** to predict the future direction of SPY.
4. **Evaluate model performance** and compare the accuracy of Logistic Regression and Random Forest models.
5. **Provide insights and recommendations** based on model predictions.

## Data Sources

- **Yahoo Finance** for historical data on:
    - S&P 500 ETF (SPY)
    - EUR/USD exchange rates
    - JPY/USD exchange rates

## Methodology

### 1. Data Collection and Preprocessing

- **Date Range**: May 1, 2019 - May 1, 2024
- **Data Download**:
    - S&P 500 ETF (SPY) prices
    - EUR/USD exchange rates
    - JPY/USD exchange rates

- **Data Cleaning and Transformation**:
    - Extract 'Adj Close' prices for SPY, EUR/USD, and JPY/USD.
    - Combine data into a single DataFrame.
    - Calculate daily percentage changes for each dataset.
    - Create directional signals for SPY (1 if price increases, 0 otherwise).
    - Handle missing values by dropping NaNs.

### 2. Data Visualization

- **Historical Prices**:
    - Line plots of SPY, EUR/USD, and JPY/USD adjusted close prices.

- **Percentage Changes**:
    - Line plots of daily percentage changes for SPY, EUR/USD, and JPY/USD.
    - Additional focus on JPY/USD fluctuations through detailed plots of historical prices and percentage changes.

### 3. Model Development

- **Features and Labels**:
    - Features: Percentage changes of EUR/USD and JPY/USD.
    - Labels: Directional signal of SPY.

- **Handling Imbalanced Data**:
    - Use SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

- **Train-Test Split**:
    - Split the balanced dataset into training (60%) and testing (40%) sets.

- **Machine Learning Models**:
    - Logistic Regression
    - Random Forest Classifier

### 4. Model Evaluation

- **Performance Metrics**:
    - Accuracy scores for both models.
    - Classification reports for both models.

### 5. Future Prediction and Insights

- **User Input**:
    - Allow user to input a date for prediction.

- **Data Fetching**:
    - Fetch historical data for the given date.
    - Calculate recent percentage changes for EUR/USD and JPY/USD.

- **Model Prediction**:
    - Predict future direction of SPY using both models.
    - Provide recommendations based on model predictions.

## Tools and Technologies

- **Python** for scripting and data processing.
- **Pandas** for data manipulation and analysis.
- **Matplotlib** for data visualization.
- **Yahoo Finance API (yfinance)** for data collection.
- **Scikit-learn** for machine learning model development.
- **Imbalanced-learn (SMOTE)** for handling imbalanced datasets.


## Expected Outcomes

1. **Comprehensive Analysis** of the impact of currency fluctuations on SPY.
2. **Trained Machine Learning Models** capable of predicting the direction of SPY.
3. **Visual Insights** through various plots highlighting historical trends and fluctuations.
4. **Actionable Recommendations** based on model predictions.


## Conclusion

This project will leverage historical financial data and machine learning techniques to provide valuable insights into the impact of currency fluctuations on the S&P 500 ETF. By developing predictive models, we aim to assist investors in making informed decisions based on currency trends.
