# Crypto Price Analysis


A data-driven analysis of historical housing prices to forecast future trends and identify top-performing ZIP codes for investment opportunities.

## Project Overview

This project analyzes the price history of 20 major cryptocurrency assets to provide institutional clients with actionable insights for developing a data-driven investment thesis. By uncovering trends, correlations, and key price drivers, the analysis aims to support informed trading strategies tailored to the unique dynamics of the crypto market. This comprehensive approach enables institutional stakeholders to optimize portfolio allocation, manage risk effectively, and identify high-value opportunities in a rapidly evolving asset class.

The analysis includes:
- Historical price trends.
- Forecasting future values using ARIMA, SARMIAX, and Prophet models.
- Visualizing growth across top assets

## Dataset

- **Source**: Kaggle Crypto Price Dataset  [view data here](https://www.kaggle.com/datasets/svaningelgem/crypto-currencies-daily-prices?resource=download&select=XRP.csv)

- **Description**: Contains historical crypto prices for major assets, including:
  - **Ticker**: ticker for each asset
  - **Open**: open price for asset on that date
  - **Close**: close price for asset
  - **Day**: Date of data

## Workflow

### Data Cleaning and Preparation:
- Removed missing values and outliers.
- Combine different csvs into one dataset 
- Put into time-series format

### Exploratory Data Analysis (EDA):
- Visualized trends and seasonal patterns in crypto price prices.
- Evaluate correlation between assets 

### Modeling:
- Used **ARIMA** and **SARIMAX** for time series forecasting.
- Implemented **Prophet** to capture trends and seasonality.

### Forecast and Results:
- Forecasted crypto prices for the next 12 months.
- Identified assets and trading strategies 

### Visualization:
- Plotted growth trends and bar charts for the top 4 crypto assets 

## Model Results

We applied multiple time series models to analyze and forecast housing prices across ZIP codes. Below are the key results:

**Models Compared**:
- **Auto-ARIMA**:  
  - Finds best parameters for each asset evaluated
  - Provides positive trading strategy but less than generic buy and hold

- **Auto-ARIMA w/ Moving Average**:  
  - Utilizes Auto-ARIMA to find best parameters and moving average trading strategy for 7d vs 30d data

- **Prophet Model**:  
  - Discovers trends in historical data
  - Utilizes RSI buy / sell signals for trades 
  - Provides returns better than the market 



## Next Steps

### 1. **Improving Models**
- **Hyperparameter Tuning**: Use grid search or Bayesian optimization to fine-tune ARIMA, SARIMAX, and Prophet models for better performance.
- **Cross-Validation**: Implement walk-forward cross-validation to evaluate model robustness over different time periods.
- **Explore Advanced Models**: Experiment with LSTM and XGBoost for capturing more complex patterns in cryptocurrency price data.

### 2. **Adding Additional Data to Feed the Model**
- **Market Sentiment**: Integrate sentiment analysis from social media or news to enhance prediction accuracy.
- **External Economic Indicators**: Add data such as interest rates, inflation, and job growth to improve model forecasts.
- **Technical Indicators**: Include additional technical indicators like MACD and Bollinger Bands to enrich the model’s feature set.

### 3. **Developing More Robust Trading Strategies**
- **Dynamic Signals**: Generate buy/sell signals based on forecasts from ARIMA, SARIMAX, or Prophet models.
- **Risk Management**: Implement stop-loss and take-profit mechanisms to limit potential losses and lock in gains.
- **Momentum Strategies**: Use short-term and long-term moving average crossovers for trend-following strategies.

### 4. **Model Monitoring & Maintenance**
- **Retraining Models Regularly**: Ensure models are retrained with the most recent data to handle market changes.
- **Real-Time Evaluation**: Continuously monitor model performance and set up alerts when performance dips.
- **Deploy for Real-Time Predictions**: Use cloud services to deploy models for real-time predictions and execution.

### 5. **Expanding & Scaling the Project**
- **Multi-Asset Strategy**: Expand strategies to more cryptocurrencies for portfolio diversification.
- **Pair Trading**: Implement pair trading strategies with highly correlated or inverse correlated assets.
- **Interactive Dashboard**: Build a dashboard for visualizing predictions, market conditions, and trading signals in real-time.


## Navigating the Git Repository
- [**price_data**](https://github.com/alecs1523/crypto_price_analysis/tree/main/price_data)
- [**README.md**](https://github.com/alecs1523/crypto_price_analysis/blob/main/README.md)
- [**crypto_price_analysis.ipynb**](https://github.com/alecs1523/crypto_price_analysis/blob/main/crypto_price_analysis.ipynb)


## Contact

**Alec Schonfeld**  
Email: [alecschonfeld15@gmail.com](mailto:alecschonfeld15@gmail.com)  
GitHub: [https://github.com/alecs1523](https://github.com/alecs1523)
