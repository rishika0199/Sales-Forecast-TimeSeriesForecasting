# Objective
Develop a data-driven sales forecasting solution using time series and causal models to predict future product demand, guide inventory planning, and improve business decision-making. The goal was to compare multiple forecasting methods and identify the best-performing model for accurate, scalable sales projections.

# Overview
This project analyzed historical sales data with strong seasonal trends and a linear pattern. The dataset was explored through time series decomposition and stationarity checks. Multiple models were applied, including:

Seasonal Naïve Model

Holt-Winters Triple Exponential Smoothing

ARIMA & SARIMA Models

Linear Regression (Causal Model)

Each model was trained and tested on partitioned datasets to evaluate accuracy, trend capture, and forecasting strength. Performance was benchmarked using MAPE and RMSE metrics. The final deployment recommendation was based on real-world forecasting reliability and simplicity.


# Key Insights

1.Linear Regression Outperformed – The regression model captured the trend and seasonality better than pure time series methods due to the dataset’s linear nature.

2.Seasonality Confirmed – Monthly seasonality was visible across all models, especially in Holt-Winters and SARIMA outputs.

3.Naïve Models Lag – While easy to implement, naive approaches were not reliable for longer horizons due to their inability to capture underlying trends.

4.Model Stability – Regression offered more stable forecasts with lower error margins across multiple windows, assuming future trends remain consistent.

5.Data Requirements – Classical models like ARIMA and SARIMA required deeper parameter tuning and data transformations (e.g., differencing) to stabilize variance and mean.



# Conclusions & Recommendations

1.Use Regression for Forecasting – With seasonal and linear patterns, linear regression is the most interpretable and accurate model for this dataset.

2.Automate Forecasts – Integrate regression logic into Excel or BI tools for business-friendly forecast execution and visualization.

3.Future Model Enhancements – For non-linear or irregular patterns, explore advanced ML models like XGBoost or Prophet.

4.Include Exogenous Variables – Enhance forecasts with external factors like marketing spend or holiday periods to refine accuracy.

5.Continuous Validation – Monitor model accuracy using rolling windows and adjust features or retrain models quarterly for reliability.e
