# 🌬️ Wind Power Generation Forecasting (Germany, 2017-2019)
### 📌 Project Overview
This project focuses on forecasting wind power generation for the last month of 2019 (December) using historical weather and wind capacity data from Germany (2017-2019). Several time series forecasting models were explored, including SARIMA, Seasonal Naïve, ETS, seasonally adjusted ARIMA, and SARIMAX.

After evaluating model performance using key error metrics, SARIMA emerged as the best-performing model for capturing seasonal and trend-based patterns in wind power generation.

### 📊 Dataset Description
The dataset contains daily measurements from 2017 to 2019, with the following key variables:

- Temperature (°C)
- Wind Capacity (installed capacity for wind power)
- Wind Generation (actual power produced)
The main objective is to predict wind generation in December 2019 based on historical patterns and relationships with other variables.

## 🔄 Project Workflow
The project follows a structured forecasting pipeline:

### 1️⃣ Data Preprocessing
✔️ Load and clean the dataset (handling missing values, converting time formats).
✔️ Perform initial transformations to ensure consistency.

### 2️⃣ Exploratory Data Analysis (EDA)
✔️ Descriptive statistics: Mean, variance, and distribution of key variables.
✔️ Time series visualization: Line plots to observe trends, seasonality, and anomalies.
✔️ Correlation analysis: Checking relationships between temperature, wind capacity, and wind generation.

### 3️⃣ Time Series Analysis
✔️ Identify seasonal patterns, stationarity, and autocorrelations using ACF & PACF plots.
✔️ Compare different forecasting approaches based on model diagnostics and performance.

### 4️⃣ Model Selection & Forecasting
Several models were tested:

- 📌 Seasonal Naïve Model (baseline model)
- 📌 ETS (Exponential Smoothing)
- 📌 Seasonally Adjusted ARIMA
- 📌 SARIMAX (ARIMA with exogenous variables)
- ✅ SARIMA (Seasonal ARIMA) – Best performing model!
### 5️⃣ Model Evaluation
Each model's performance was evaluated using:

Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
Mean Absolute Percentage Error (MAPE)
- SARIMA provided the most accurate and stable forecasts, capturing seasonal effects and trends more effectively than other models.

### 🚀 Conclusion
🔹 After testing multiple forecasting methods, SARIMA outperformed all other models in predicting wind power generation.
🔹 The model effectively captures seasonality and trend, leading to reliable December 2019 forecasts.
🔹 The forecasted wind power generation values from SARIMA are displayed as follows (see results section).

### 🛠️ Technologies Used
Python 3.x
Pandas
NumPy
Statsmodels
Matplotlib & Seaborn
Scikit-learn

### 🔧 Installation & Usage
Clone the repository and install dependencies:

- git clone https://github.com/Indeewarib/windforcast.git  
- cd windforcast 
- Run the Jupyter Notebook:
jupyter notebook wind_forecast.ipynb  

### 📌 Future Improvements
🔹 Incorporate deep learning approaches like LSTMs or Prophet for further analysis.
🔹 Extend the dataset to include more recent data for better generalization.
🔹 Explore external factors such as weather conditions beyond temperature (e.g., wind speed).