# 📈 Zomato Stock Price Forecasting (SET-B)

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

# 📂 Project Structure
│
├── 📓 Time-Series Forecasting – Stock Prices.ipynb   # Main notebook
├── 📄 Time-Series Forecasting – Stock Prices(SET-B).pdf  # Assessment instruction
├── 📊 zomato_Stock_Prices.csv                        # Dataset used
└── 📘 README.md                                      # Documentation

# ⚙️ Technologies Used

* Python 3.10+
* pandas, numpy – Data handling & preprocessing
* matplotlib, seaborn – Visualization
* statsmodels – ARIMA model
* prophet – Time-series forecasting
* scikit-learn – Evaluation metrics

# 🔍 Workflow Summary
1. Data Preprocessing

* Loaded the Zomato stock dataset and parsed Date and Close columns.
* Handled missing values, checked stationarity, and applied differencing where needed.
* Performed train-test split for rolling forecast evaluation.

2. Model Development

* ARIMA Model: Tuned (p, d, q) parameters using AIC minimization.
* Prophet Model: Configured for trend and seasonality components.

3. Evaluation Metrics

The models were compared using RMSE (Root Mean Squared Error) and MAPE (Mean Absolute Percentage Error).
| Model       | RMSE       | MAPE        |
| ----------- | ---------- | ----------- |
| **ARIMA**   | **2.5433** | **2.5279%** |
| **Prophet** | **5.3216** | **6.1375%** |

# 📊 Interpretation:

* ARIMA achieved lower RMSE and MAPE, indicating higher accuracy for short-term prediction.
* Prophet performed reasonably well but was slightly less precise for this dataset.

# 📈 Visual Results

* Trend Analysis Plot: Showed clear non-stationary upward movement.
* ARIMA Forecast Plot: Captured short-term fluctuations accurately.
* Prophet Forecast Plot: Modeled long-term trend and seasonal components.
* Rolling Window Forecast: Demonstrated stable ARIMA performance over multiple periods.
(All plots are available within the Jupyter notebook.)

# 🗒️ Summary of Findings

* The ARIMA model generalized better for Zomato’s short-term stock movements.
* Prophet provided better interpretability but slightly higher forecast error.

* Combining both approaches or extending with hybrid models (ARIMA-Prophet or LSTM) 
could further improve accuracy in future iterations.

👤 Author

Zubayer Hasan
Machine Learning Enthusiast
📧 zubayerhasan12345@gmail.com
📅 25 October 2025
