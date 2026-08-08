# Netflix Stock Price Forecasting Using ARIMA

## 📌 Project Overview

In this project, I used the **ARIMA model** to predict Netflix's adjusted closing stock price.

The main goal was to understand how time-series forecasting works and see how well ARIMA can predict stock prices.

## 🎯 Objectives

* Clean the Netflix stock data
* Understand the stock-price trend
* Check whether the data is stationary
* Make the data stationary using differencing
* Study ACF and PACF
* Compare different ARIMA models
* Select the best model
* Predict Netflix stock prices
* Check the model's performance

## 🛠️ Tools Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Statsmodels
* Scikit-learn
* Google Colab

## 📊 Dataset

The dataset contains Netflix stock-price data from **2018 to 2022**.

It contains:

* Date
* Open
* High
* Low
* Close
* Adjusted Close
* Volume

I used **Adjusted Close** as the main value for forecasting.

## 🔍 What I Did

### 1. Data Cleaning

I loaded the Netflix dataset and removed the columns that were not needed.

I also converted the `Date` column into the correct date format.

### 2. Data Visualization

I created a graph to see how Netflix's stock price changed over time.

### 3. Stationarity Check

I used the **ADF test** to check whether the data was stationary.

The original data was **not stationary**.

### 4. Seasonal Decomposition

I used decomposition to understand the **trend, seasonality, and residuals** in the data.

### 5. Differencing

I applied first-order differencing to make the data stationary.

After differencing, the ADF test showed that the data had become **stationary**.

### 6. ACF and PACF

I used ACF and PACF plots to understand the data and help choose the ARIMA parameters.

### 7. Train-Test Split

I kept the last **30 days** for testing.

The remaining data was used for training.

### 8. ARIMA Models

I tested different ARIMA models and compared their performance using:

* MAE
* RMSE

The model with the lowest RMSE was selected.

## 📈 Results

The final model achieved approximately:

* **MAE: 109.35**
* **RMSE: 139.08**

The results show that the predictions were not very close to the actual Netflix stock prices.

## 🧠 My Understanding

I used ARIMA to predict Netflix's adjusted closing price.

The original data was not stationary, so I used first-order differencing. After differencing, the data became stationary.

I compared different ARIMA models and selected the model with the lowest RMSE.

The model was able to learn some patterns from the data, but the predictions were not accurate enough for reliable stock-price prediction.

Stock prices can change because of many outside factors, which are not included in this model.

## 📝 Conclusion

ARIMA is a good model for learning and understanding **time-series forecasting**.

However, it is not enough for accurate real-world stock-price prediction.

In the future, I can try models such as **SARIMAX or Machine Learning models** and use additional features like trading volume and market trends.

## 📚 What I Learned

Through this project, I learned:

* Data cleaning
* Time-series analysis
* ADF test
* Stationarity
* Differencing
* Seasonal decomposition
* ACF and PACF
* ARIMA
* Model comparison
* MAE and RMSE
* Forecasting

## 🚀 Google Colab

I created this project using Google Colab.

👉 [**Open Netflix Stock Price Forecasting Project in Google Colab**](https://colab.research.google.com/drive/1meueJwsfSA9hg5OS8NgNOey68MlLVhD5?usp=sharing)

## 📁 Project Files

* `netflix_stock_forecasting_arima.ipynb` — Project notebook
* `README.md` — Project information
* `stock.csv` — Netflix stock dataset

## ⚠️ Limitations

Stock prices are affected by many external factors.

Because of this, the model may not always give accurate predictions.

This project is mainly for **learning and understanding time-series forecasting**.

## 👨‍💻 Author

**Shaheen Khan**
