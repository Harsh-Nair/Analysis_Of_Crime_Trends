# Analysis_Of_Crime_Trends

## 📄 Project Overview
This project focuses on the analysis, forecasting, and understanding of crime patterns in the city of Chicago from 2001 to 2017.  
It leverages machine learning models (LSTM, Prophet, XGBoost) and statistical methods to uncover insights related to:

- Crime volume trends over time
- Crime hotspots and geospatial patterns
- Impact of external events (holidays) on crime rates
- Crime type prediction using classification models
- Anomaly detection to identify unusual spikes in crime

---

## 🔍 Objectives
- **Time Series Forecasting:** Predict future crime volumes using LSTM and Prophet models.
- **Geospatial Analysis:** Identify and visualize crime hotspots using KDE.
- **Crime Type Prediction:** Build a classifier (XGBoost) to predict the type of crime based on features like location, district, and FBI code.
- **Anomaly Detection:** Detect abnormal crime spikes in different districts.
- **Holiday Impact Analysis:** Evaluate if crime rates differ significantly between holidays and non-holidays using statistical tests.

---

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy, Seaborn, Scikit-learn, Matplotlib)
- **Machine Learning:** XGBoost, SMOTE Oversampling
- **Deep Learning:** LSTM (TensorFlow/Keras)
- **Time Series Modeling:** Facebook Prophet
- **Statistical Analysis:** T-Test (Scipy)
- **Geospatial Analysis:** Kernel Density Estimation (KDE)
- **Anomaly Detection:** STL Decomposition (Seasonal-Trend decomposition)

---

## 📊 Key Results

| Analysis Area             | Method/Model              | Key Insight |
|:---------------------------|:---------------------------|:------------|
| Crime Volume Forecasting    | LSTM, Prophet               | Seasonal trends captured; future crime rates forecasted |
| Crime Hotspots              | KDE (Geospatial Heatmaps)   | Persistent hotspots in central districts |
| Crime Type Prediction       | XGBoost Classifier          | Achieved high accuracy (~86%) after balancing |
| Anomaly Detection           | STL Decomposition           | Detected abnormal spikes during holidays and specific events |
| Holiday Impact on Crimes    | T-Test                      | ✅ Statistically significant lower crime rates on holidays |

---

## 📈 Forecasting
- **LSTM and Prophet** models were trained on daily crime counts.
- **Evaluation Metrics:**
  - **RMSE:** (Root Mean Squared Error) measured prediction accuracy.
  - **MAE:** (Mean Absolute Error) provided another performance indicator.
- **Conclusion:**  
  Prophet provided slightly better RMSE for short-term forecasts, while LSTM was more flexible for seasonality.

---

## 📉 Anomaly Detection
- Applied **STL Decomposition** to extract trend, seasonality, and residuals from the time series.
- Detected **spikes** that matched:
  - Major public events
  - Holidays
  - Weather extremes

---

## 📑 Files and Structure

```bash
├── README.md
├── datasets/
│   ├── Chicago_Crimes_Cleaned.csv
│   ├── US_Holiday_Dates.csv
├── notebooks/
│   ├── CrimeRates.ipynb         # Full crime forecasting & analysis
│   ├── CrimeType.ipynb        # Classification model (XGBoost) + holiday impact analysis
├── outputs/
│   ├── Forecast plots
│   ├── Hotspot heatmaps
│   ├── Anomaly detection graphs
