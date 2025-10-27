# 🌦️ Weather Data Analysis and Prediction

## 📘 Project Overview

This project focuses on analyzing **historical weather data** and building a **machine learning model** to predict future temperature trends.  
It serves as an excellent introduction to **time series analysis**, **data visualization**, and **regression modeling** using Python.  

By understanding the relationships between temperature, humidity, pressure, and other atmospheric variables, we can gain insights into how weather patterns change over time.

---

## 🎯 Objectives

1. Perform **Exploratory Data Analysis (EDA)** on the weather dataset.
2. Visualize and understand trends in temperature, humidity, and pressure.
3. Identify correlations between weather variables.
4. Build a **machine learning model** to predict temperature using other features.
5. Evaluate model performance and interpret results.

---

## 🧩 Dataset Description

The dataset contains **hourly weather observations** including temperature, humidity, wind speed, visibility, and pressure.

| Column Name        | Description                          | Example Value |
|--------------------|--------------------------------------|----------------|
| Date/Time          | Timestamp of observation              | 2012-01-01 00:00 |
| Temp_C             | Temperature in Celsius                | -1.8 |
| Dew Point Temp_C   | Dew point temperature in Celsius      | -3.9 |
| Rel Hum_%          | Relative humidity in %                | 86 |
| Wind Speed_km/h    | Wind speed in km/h                    | 4 |
| Visibility_km      | Visibility distance in km             | 8.0 |
| Press_kPa          | Atmospheric pressure in kPa           | 101.24 |
| Weather            | Weather condition (e.g., Fog, Snow)   | Fog |

**Rows:** 8784  
**Columns:** 8  
**Missing Values:** None ✅  

---

## 🧠 Technologies Used

- **Programming Language:** Python  
- **Data Analysis Libraries:** Pandas, NumPy  
- **Visualization Tools:** Matplotlib, Seaborn  
- **Machine Learning:** Scikit-learn  
- **Model Used:** Linear Regression  

---

## ⚙️ Steps in the Project

### 1️⃣ Data Preprocessing
- Convert `Date/Time` column into proper datetime format.
- Check for missing values and data consistency.
- Extract time-related features like **year, month, hour** for trend analysis.

### 2️⃣ Exploratory Data Analysis (EDA)
- Descriptive statistics and data distribution.
- Line plots for temperature trends over time.
- Correlation heatmap to visualize relationships between variables.
- Monthly average temperature trends.

### 3️⃣ Visualization
- **Temperature vs Time:** Observe daily and seasonal variations.
- **Humidity vs Temperature:** Understand inverse relationship.
- **Pressure Trends:** Analyze atmospheric pressure over time.
- **Correlation Heatmap:** Identify which variables affect temperature most.

### 4️⃣ Model Building
We used a **Linear Regression** model to predict temperature (`Temp_C`) based on:


### 5️⃣ Model Evaluation
We split data into:
- **Training set:** 80%
- **Testing set:** 20%

**Metrics used:**
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

These metrics help measure how well the model predicts temperature trends.

---

## 📊 Insights and Observations

### 🔹 1. Temperature Trends
- Clear **seasonal pattern** observed — lower temperatures in winter months and higher during summer.
- Sudden temperature drops correspond to rainy or snowy weather.

### 🔹 2. Relationship Insights
- **Temperature and Dew Point**: Strong positive correlation (~0.9).  
  → When dew point rises, temperature tends to increase.
- **Temperature and Humidity**: Weak inverse correlation.  
  → Higher humidity often occurs when temperatures are lower.
- **Pressure and Temperature**: Slight negative correlation.  
  → Low pressure generally corresponds to cloudy or rainy weather.

### 🔹 3. Model Performance
- The model captures general temperature patterns quite well.
- **R² Score ~ 0.95**, indicating strong predictive performance.
- Slight prediction deviations may occur during extreme weather conditions.

---

## 🧾 Conclusion

- Temperature is primarily influenced by **dew point**, **humidity**, and **pressure**.
- Seasonal and daily variations can be captured effectively using regression techniques.
- This project demonstrates the practical application of **machine learning** in environmental science.
- With more advanced models (e.g., Random Forest, LSTM), prediction accuracy could be further improved.

---

## 🚀 Future Improvements

1. Implement **Time Series Forecasting (ARIMA, Prophet, or LSTM)** for trend prediction.
2. Incorporate **real-time weather data** using APIs.
3. Build a **Streamlit Dashboard** to visualize predictions interactively.
4. Expand the dataset with additional features (e.g., precipitation, UV index).

---

🏁 Final Thoughts

This project not only showcases data analysis and visualization skills but also demonstrates the power of simple regression models in understanding real-world phenomena like weather.
It’s a great foundation for moving into more advanced forecasting techniques and interactive applications.

Author: Amit Yadav
Project Title: Weather Data Analysis and Prediction
Date: October 2025
Tools: Python, Pandas, Matplotlib, Seaborn, Scikit-learn
Dataset: Weather Data.csv
