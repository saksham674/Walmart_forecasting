# 🛒 Walmart Sales Forecasting & Analysis using Prophet

## 📌 Overview
This project focuses on analyzing Walmart retail sales data and building a time-series forecasting model to predict future weekly sales.

The analysis includes data cleaning, outlier removal, correlation analysis, and store-level forecasting using Facebook Prophet.

---

## 📊 Dataset
- Walmart sales dataset
- ~6435 records
- Features include:
  - Store
  - Date
  - Weekly Sales
  - Temperature
  - Fuel Price
  - CPI
  - Unemployment
  - Holiday Flag

---

## ⚙️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Plotly (for interactive visualizations)
- Statsmodels
- Facebook Prophet

---

## 🔍 Key Steps & Work Done

### 1. Data Preprocessing
- Converted `Date` column into datetime format
- Checked for:
  - Missing values
  - Duplicate records
- Removed outliers using **IQR (Interquartile Range)** method on:
  - Weekly Sales
  - Temperature
  - Unemployment

---

### 2. Exploratory Data Analysis (EDA)
- Box plots for all features to detect outliers
- Scatter plots and regression plots to analyze relationships
- Key analysis:
  - Weekly Sales vs Unemployment
  - Weekly Sales vs Temperature
  - Weekly Sales vs CPI

---

### 3. Correlation Analysis
- Calculated correlations between:
  - Sales & Unemployment
  - Sales & CPI
- Performed **store-wise correlation analysis**
- Identified:
  - Most affected stores
  - Least affected stores

---

### 4. Time Series Analysis
- Resampled data weekly
- Performed **seasonal decomposition**:
  - Trend
  - Seasonality
  - Residuals

- Created:
  - Monthly sales trends
  - Weekly trends across year

---

### 5. Store Performance Analysis
- Identified:
  - Top-performing stores
  - Worst-performing stores
- Compared total sales across stores

---

### 6. Stationarity Check
- Used **ADF (Augmented Dickey-Fuller Test)**
- Applied:
  - Log transformation
  - Differencing
  - Rolling mean & standard deviation

---

### 7. Visualization
- Line plots for trends
- 3D plots (Sales vs Unemployment vs Store)
- Store-wise sales comparison using Plotly

---

### 8. Forecasting using Prophet
- Built **individual Prophet models for each store**
- Steps:
  - Renamed columns (`ds`, `y`)
  - Enabled weekly seasonality
  - Trained model per store
  - Generated future predictions

---

## 📈 Results & Insights
- Sales show clear seasonal patterns
- Certain stores are highly sensitive to unemployment and CPI
- Significant variation in performance across stores
- Prophet successfully generated future sales forecasts


---

## 📷 Visualizations Included
- Box plots (outlier detection)
- Regression plots
- Seasonal decomposition graphs
- Store-wise comparison charts
- Forecast plots

---

## 🚀 Future Improvements
- Add evaluation metrics (RMSE, MAE)
- Use LSTM for deep learning forecasting
- Deploy using Streamlit dashboard
- Add feature engineering for better accuracy

---

## 🔗 Project Structure
walmart-sales-forecasting/
│
├── Walmart.ipynb
├── Walmart_DataSet.csv
├── README.md


---

## 👨‍💻 Author
Saksham Goel  
Aspiring AI Engineer
