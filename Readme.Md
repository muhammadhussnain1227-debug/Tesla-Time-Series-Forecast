# 📈 Tesla Stock Price Forecasting

This project focuses on **forecasting Tesla (TSLA) stock prices** using a comprehensive comparison of **classical time series models**, **machine learning models**, and **deep learning architectures**.  
The goal is to evaluate different forecasting approaches under a unified preprocessing and evaluation pipeline and identify the best-performing model using **RMSE (Root Mean Squared Error)**.

---

## 🚀 Project Objectives

- Perform **end-to-end time series forecasting** on Tesla stock price data
- Apply and compare:
  - Classical time series models
  - Classical machine learning models
  - Deep learning models
- Follow **proper time series preprocessing steps**
- Evaluate all models using a **common metric (RMSE)**
- Identify the **lowest-error forecasting model**

---

## 📊 Dataset

- **Stock:** Tesla Inc. (TSLA)
- **Type:** Univariate time series
- **Target Variable:** Closing Price
- **Frequency:** Daily stock prices
- **Source:** Public stock market data (e.g., Yahoo Finance)

---

## 🔧 Preprocessing Pipeline

All models follow **standard time series preprocessing steps**, including:

- Handling missing values
- Sorting data chronologically
- Date-time indexing
- Train-test split based on time (no shuffling)
- Stationarity checks (ADF test)
- Differencing (where required)
- Scaling (for ML & DL models)
- Lag feature generation
- Sliding window technique (for deep learning)

This ensures **fair comparison** across all models.

---

## 🧠 Models Implemented

### 📌 Classical Time Series Models

1. **AR (AutoRegressive)**
2. **MA (Moving Average)**
3. **ARMA**
4. **ARIMA**
5. **SARIMA (Seasonal ARIMA)**

---

### 🤖 Classical Machine Learning Models

1. **Random Forest Regressor**
2. **Stochastic Gradient Boosting**
3. **Support Vector Machine (SVM)**

---

### 🧬 Deep Learning Models

1. **Basic Neural Network (ANN)**
2. **LSTM (Long Short-Term Memory)**
3. **GRU (Gated Recurrent Unit)**

---

## 📏 Evaluation Metric

All models are evaluated using:

### **RMSE (Root Mean Squared Error)**

\[
RMSE = \sqrt{\frac{1}{n}\sum_{i=1}^{n}(y_i - \hat{y}_i)^2}
\]

- Lower RMSE indicates **better forecasting performance**
- Same evaluation strategy applied to all models

---

## 🏆 Results Summary

| Model Type | Model Name | RMSE |
|-----------|----------|------|
| Time Series | **MA (Moving Average)** | **10.51 (Best)** |
| Time Series | AR | Higher |
| Time Series | ARMA | Higher |
| Time Series | ARIMA | Higher |
| Time Series | SARIMA | Higher |
| ML | Random Forest | Higher |
| ML | Gradient Boosting | Higher |
| ML | SVM | Higher |
| DL | ANN | Higher |
| DL | LSTM | Higher |
| DL | GRU | Higher |

✅ **Lowest RMSE achieved by the Moving Average (MA) model**

---

## 🔍 Key Insights

- Simpler statistical models can outperform complex ML/DL models in certain time series problems
- Overfitting risk increases with complex models on limited data
- Proper preprocessing is more impactful than model complexity
- MA model captured short-term price dynamics effectively

---

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib / Seaborn**
- **Statsmodels**
- **Scikit-learn**
- **TensorFlow / Keras**

---


---

## 📌 Conclusion

This project demonstrates that **classical time series models**, when applied correctly, can outperform advanced machine learning and deep learning models for stock price forecasting.  
The **Moving Average (MA)** model achieved the **lowest RMSE of 10.51**, making it the most accurate model in this study.

---

## 👤 Author

**Muhammad Hussnain**  
Time Series Forecasting | Machine Learning | Deep Learning

---

## ⭐ If you like this project

Give it a ⭐ on GitHub — it helps a lot!
