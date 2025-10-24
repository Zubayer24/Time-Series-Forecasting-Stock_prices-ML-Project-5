📈 Zomato Stock Price Forecasting (SET-B)

🧠 Project Overview
This project was completed as part of the DataSynthis ML Job Assessment (SET-B).
The goal was to forecast Zomato’s future stock prices using time-series forecasting models and compare traditional statistical methods with modern machine learning techniques.

🎯 Objectives

1. Implement a traditional statistical model (ARIMA).
2. Implement a machine learning model (Prophet).
3. Evaluate both models using rolling window forecasting.
4. Compare models using performance metrics (RMSE, MAPE).
5. Discuss which model generalizes better.

📂 Project Structure
│
├── 📓 Time-Series Forecasting – Stock Prices.ipynb   # Main notebook
├── 📄 Time-Series Forecasting – Stock Prices(SET-B).pdf  # Assessment instruction
├── 📊 zomato_Stock_Prices.csv                        # Dataset used
└── 📘 README.md                                      # Documentation

⚙️ Technologies Used

* Python 3.10+
* pandas, numpy – Data handling & preprocessing
* matplotlib, seaborn – Visualization
* statsmodels – ARIMA model
* prophet – Time-series forecasting
* scikit-learn – Evaluation metrics

🔍 Workflow Summary
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

📊 Interpretation:

* ARIMA achieved lower RMSE and MAPE, indicating higher accuracy for short-term prediction.
* Prophet performed reasonably well but was slightly less precise for this dataset.

📈 Visual Results

* Trend Analysis Plot: Showed clear non-stationary upward movement.
* ARIMA Forecast Plot: Captured short-term fluctuations accurately.
* Prophet Forecast Plot: Modeled long-term trend and seasonal components.
* Rolling Window Forecast: Demonstrated stable ARIMA performance over multiple periods.
(All plots are available within the Jupyter notebook.)

🗒️ Summary of Findings

* The ARIMA model generalized better for Zomato’s short-term stock movements.
* Prophet provided better interpretability but slightly higher forecast error.

* Combining both approaches or extending with hybrid models (ARIMA-Prophet or LSTM) 
could further improve accuracy in future iterations.

👤 Author

Zubayer Hasan
Machine Learning Enthusiast
📧 zubayerhasan12345@gmail.com
📅 25 October 2025
