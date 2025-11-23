# 📈 Zomato Stock Price Forecasting Using Machine Learning 

# 🧠 Project Overview
The objective is to predict Zomato’s future stock prices using traditional statistical models and modern machine-learning forecasting methods, followed by model comparison and business impact analysis.

# 🎯 Problem Summary (Business Context)

Accurate stock forecasting is essential for investment decisions, portfolio risk management, and financial planning. Even small price fluctuations influence trading strategies and investor sentiment.
This project builds a predictive pipeline for Zomato’s stock, comparing ARIMA and Prophet models to determine which model provides more reliable short-term forecasts in real-world market environments.

# What I Did (Approach)
✅ Data Cleaning & Preprocessing

- Loaded and parsed Zomato stock price dataset
- Converted date column to datetime index
- Handled missing/duplicate values
- Checked stationarity with ADF test
- Applied differencing for non-stationary behavior
- Conducted trend & seasonality analysis

✅ Feature Engineering

- Lag-based transformations for ARIMA
- Trend & seasonal components for Prophet

✅ Model Development

- ARIMA: Tuned (p, d, q) parameters using AIC
- Prophet: Configured for additive trend & seasonality

✅ Rolling Window Forecasting

- Simulated real trading scenarios
- Generated forecast for multiple rolling windows
- Collected performance metrics for each iteration

✅ Model Evaluation

Compared models with:
- RMSE (Root Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)
-Included visual forecast comparisons




```md
## Project Structure


├── Time-Series Forecasting – Stock Prices.ipynb      # Main notebook
├── README.md                                         # Project documentation
├── zomato_Stock_Prices.csv                           # Dataset

```

# Key Results
📊 Model Performance Table:

| Model     | RMSE       | MAPE        |
| --------- | ---------- | ----------- |
| **ARIMA** | **2.5433** | **2.5279%** |
| Prophet   | 5.3216     | 6.1375%     |

📈 Visual Outputs Included

- Historical trend analysis
- ARIMA forecast vs actual
- Prophet forecast vs actual
- Prophet trend/seasonality components
- Rolling window performance plots

📌 Interpretation

- ARIMA outperformed Prophet with significantly lower error.
- ARIMA captured short-term fluctuations more accurately.
- Prophet provided smoother long-term trends but struggled with volatility.
- Rolling window evaluation proved ARIMA’s better generalization.

4. Business Impact
💼 Improved Investment Decisions
Short-term price forecasting helps traders optimize entry/exit timing.

📉 Reduced Market Risk
Accurate predictions reduce uncertainty and support risk-aware portfolio optimization.

📊 Better Stakeholder Insights
Prophet’s trend component helps long-term investors and management understand growth trajectory.

🔍 Model Reliability
Rolling-window evaluation ensures the model is dependable when deployed in real-world trading systems.

# ⚙️ Technologies Used
* Python 3.10+
* pandas, numpy – Data handling & preprocessing
* matplotlib, seaborn – Visualization
* statsmodels – ARIMA model
* prophet – Time-series forecasting
* scikit-learn – Evaluation metrics

# Summary of Findings
- ARIMA is the optimal model for short-term Zomato stock forecasting.
- Prophet provides valuable insights but has higher prediction error.
- Hybrid and deep-learning approaches (ARIMA + Prophet or LSTM) could enhance future versions.

👤 Author

Zubayer Hasan
Machine Learning Enthusiast
📧 zubayerhasan12345@gmail.com
📅 25 October 2025
