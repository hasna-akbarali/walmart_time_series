# 📈 Time Series Analysis of Walmart Stock 📊

## Introduction
Welcome to the rollercoaster ride of Walmart stock prices! 🎢 This project dives deep into the world of stock price movements, forecasting, and data wizardry. Buckle up as we journey through data preparation, decomposition, stationarity testing, and the ultimate showdown of forecasting models.

## Data Preparation 🧹
- **Data Source:** 🕵️‍♂️ Sourced historical price data from 2014-06-03 to 2024-06-04 using the magical powers of `yfinance`.
- **Data Cleaning:** 🧼 Checked for pesky null values or duplicates. Spoiler: there were none!
- **Feature Engineering:** 🛠️ Added cool columns like '30-Day Moving Average', '90-Day Moving Average', '150-Day Moving Average', '210-Day Moving Average', 'Close First Difference', and 'Close 12 Difference' to supercharge our analysis.

## Exploratory Analysis 🔍
- **Visual Treats:** 🎨 Feast your eyes on the graphical representations of Open, High, Low, Close, Adj Close, Volume over the past decade.
- **Stock Price Highlights:**
  - 📈 **Highest Closing Price:** $65.379 on 2024-05-24.
  - 📉 **Lowest Closing Price:** $33.18 on 2019-05-09.
- **Year-End Extravaganza:** 🎉 Check out how Walmart stock has wrapped up each year over the past 10 years.
- **Quarter-Start Insights:** 🗓️ Analyze the stock performance at the start of each quarter.
- **Moving Averages Galore:** 📊 Plot and admire the 30-Day, 90-Day, 150-Day, and 210-Day moving averages.

## Time Series Decomposition 🔬
- **Trend, Seasonality, Residuals:** 🧩 Unraveled using the mystical powers of STL decomposition.

## Stationarity Testing 🧪
- **ADF Test:** 📝 Conducted the Augmented Dickey-Fuller test to check for stationarity. Spoiler: It wasn't stationary.
- **Transformation Magic:** ✨ Applied differencing to achieve the zen state of stationarity. First differencing did the trick! Also checked 12th differencing for seasonality.

## Forecasting Model Development 🧠
- **ARIMA:** 📉 The classic ARIMA model with pdq values from PACF and ACF graphs.
  - **Performance:** Not so great (MAE: 6.673, RMSE: 7.711). ARIMA, you tried your best!

- **SARIMAX:** 🔄 The seasoned SARIMAX model with pdq and seasonality values from PACF and ACF graphs.
  - **Performance:** Improved results (MAE: 4.51, RMSE: 5.42). Nice try, SARIMAX!

- **Prophet:** 🔮 Utilized Prophet for forecasting and plotted the magical forecast.
  - **Performance:** Impressive (MAE: 1.33, RMSE: 2.09). Way to go, Prophet!

- **LSTM:** 🤖 Enter the neural network! Implemented LSTM and plotted the forecast.
  - **Performance:** Superstar results (MAE: 1.33, RMSE: 2.09). Predicted Close Price on 2023-12-01: $50.82 (Actual: $51.45), with approximately 1.22% error. LSTM, you rock!

## Conclusion 🎬
- This wild ride shows how different forecasting models stack up against Walmart's stock data.
- The LSTM model is the undisputed champion, providing the most accurate predictions.

## Recommendations 🔮
- Future explorers, consider:
  - Further hyperparameter tuning of the LSTM model.
  - Incorporating additional external variables (e.g., economic indicators) for even more accuracy.
  - Regular updates and retraining of models to stay sharp with new data.
