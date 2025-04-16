# 🛍️ Retail Sales Forecasting | Data Science Internship @ Wiseanalytics

Forecasting daily sales for a major retail chain in Ecuador using advanced feature engineering, machine learning, and time series modeling techniques. This project was completed as part of my Data Science Internship at **Wiseanalytics**, with the goal of generating actionable insights and boosting inventory planning efficiency.

---

## 📌 Project Objective

Build a robust sales forecasting model using historical transactional data, promotions, oil prices, store information, and holiday events. The final solution identifies key business drivers and offers strategic recommendations.

---

## 🔄 Workflow Overview

### 🔹 Part 1: Data Processing & Feature Engineering
- Merged multiple datasets: `train`, `test`, `stores`, `oil`, and `holidays_events`.
- Cleaned missing oil prices using linear interpolation.
- Engineered features:
  - **Temporal:** day, month, year, dayofweek, weekofyear
  - **Events:** holidays, promotions, paydays, earthquake
  - **Lag & Rolling Stats:** lag-7, lag-30, rolling mean & std
  - **Store & Cluster Level Insights:** average store sales, top-performing families

### 🔹 Part 2: Modeling & Evaluation
- **Models Used:**
  - 📊 Baseline Naïve Model
  - 🌲 Random Forest Regressor
  - ⚡ XGBoost Regressor
  - 🔁 ARIMA (for individual series)
  - 🤖 LSTM (deep learning-based time series model)
- **Evaluation Metrics:** RMSE, MAPE, R² Score
- **Validation:** Time-based split using the last 30 days of data

---

## 📈 Results & Insights

| Model        | RMSE ↓  | MAPE ↓ | R² ↑  |
|--------------|---------|--------|-------|
| Baseline     | X.XX    | XX%    | X.XX  |
| RandomForest | X.XX    | XX%    | X.XX  |
| XGBoost ✅    | **X.XX**| **XX%**| **X.XX**|

- **Best Model:** XGBoost delivered the best performance across all metrics.
- **Key Sales Drivers:**
  - Holidays and promotional campaigns
  - Oil price fluctuations (macro impact)
  - Paydays (15th and end of month)
- **Recommendations:**
  - Align promotions with high-demand windows
  - Monitor oil prices to adjust economic forecasts
  - Focus marketing on top-selling product families per cluster

---

## 📊 Visualizations

- Total sales trends over time
- Sales patterns around holidays
- Oil price correlation with sales
- Actual vs. predicted sales comparison
- Feature importance plot (XGBoost)

---

## 🧠 Skills Demonstrated

- ✅ Data Cleaning & Feature Engineering
- ✅ Time Series Analysis
- ✅ Supervised Learning (Sklearn, XGBoost)
- ✅ Deep Learning with LSTM (Keras)
- ✅ Model Evaluation & Visualization
- ✅ Business Insight Generation
