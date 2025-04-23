# Analysis_Of_Crime_Trends

# Chicago Crime Rate Analysis and Forecasting (2001-2017)

## 📌 Introduction

This project analyzes crime data from Chicago between 2004 and 2021. It involves:

- **Data Cleaning and Preparation**
- **Exploratory Data Analysis (EDA)**
- **Forecasting Crime Rates** using LSTM, Prophet, and XGBoost
- **Anomaly Detection** to find unusual spikes
- **Holiday Impact Analysis** using Statistical Testing (T-Test)

---
## 🛠️ Tech Stack

**Languages & Libraries:**

- 🐍 Python (Pandas, NumPy)
- 📊 Visualization (Matplotlib, Seaborn)
- 🤖 Machine Learning (XGBoost, Scikit-learn, SMOTE)
- 🔮 Deep Learning (TensorFlow, LSTM)
- 📈 Time Series Forecasting (Facebook Prophet)
- 🧪 Statistical Analysis (SciPy T-Test)
- 🌍 Geospatial Analysis (Kernel Density Estimation)

---

## 📂 Project Structure

```bash
📦 Chicago-Crime-Analysis
 ┣ 📜 README.md
 ┣ 📁 datasets/
 ┃ ┣ 📄 Chicago_Crimes_Cleaned.csv
 ┃ ┣ 📄 US_Holiday_Dates.csv
 ┣ 📁 notebooks/
 ┃ ┣ 📓 CrimeRates.ipynb (Forecasting + Analysis)
 ┃ ┣ 📓 chicago-set2.ipynb (Classification + Holidays Analysis)
 ┣ 📁 outputs/
 ┃ ┣ 📈 Forecast Plots
 ┃ ┣ 🗺️ Hotspot Heatmaps
 ┃ ┣ 🚨 Anomaly Detection Graphs

```
---

## 📚 Datasets Used

- **Crime Data:** Chicago Crimes Cleaned (2001-2017)
- **US Holiday Data:** US Holiday Dates (2004-2021)

---

## 🔍 Analysis and Modeling

### 📈 Forecasting
- **Models Used:**
  - **LSTM:** Captured complex time series patterns.
  - **Prophet:** Handled trend and seasonality effectively.
  - **XGBoost:** Focused on crime type classification.
  - **IsolationForest:** For anomaly detection.
  
- **Performance Metrics:**
  - **LSTM:** MAE = 24.92
  - **Prophet:** MAE = 27.45
  - (Lower MAE indicates better performance.)
  - **XGBoost:** Accuracy = 94.05%

- **Forecasting Summary:**  
  LSTM slightly outperformed Prophet. Both models successfully captured seasonal crime trends and forecasted future crime rates over the next year.

---

### 🚨 Anomaly Detection
- **Technique:** STL Decomposition
- **Findings:**
  - Detected multiple crime spikes that aligned with major public events or holidays.
  - Anomalies mostly occurred around national holidays, large events, and certain weekends.

---

### 📅 Holiday Impact Analysis
- **Method:** T-Test (Independent Samples)
- **Result:**
  - P-value < 0.05 → **Statistically Significant**
  - ✅ Crime rates were significantly lower on holidays compared to non-holidays.

---

## ⚡ Key Results Summary

- **Forecast Models:** LSTM performed best in accuracy.
- **Crime Patterns:** Clear seasonal trends observed — crime rates higher during summer.
- **Anomalies:** Significant spikes aligned with major events and holiday weekends.
- **Holiday Analysis:** Holidays had statistically fewer crimes.

---

## 🧹 Limitations

- Some anomalies could not be explained only by holidays — other external factors (e.g., weather, sports events) were not modeled.
- Forecasting accuracy could improve with inclusion of external regressors (e.g., weather, unemployment rates).

---

## 🚀 Future Work

- Integrate external data sources like weather conditions, socio-economic factors.
- Deploy models into a real-time dashboard.
- Experiment with Transformer-based time series models (e.g., TFT, Informer).

---

## 👨‍💻 Author

- **Ananya Tiwari** 
  [Linkedln](https://linkedin.com/in/ananya-tiw)

---

> _"Data analysis is the art of making sense out of chaos."_
