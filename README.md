# BDA600 Capstone: San Francisco Police Incident Analysis (2020–2024)

**Authors:** Eddie Rosas & Swikriti Joshi 
**Program:** M.S. Big Data Analytics, San Diego State University  
**Course:** BDA 600 – Capstone Seminar  

[🌐 Live Project Site](https://erosas9172.github.io/BDA600_Capstone/) •
[📄 Final Report (PDF)](BDA600_Final_Project_Report.pdf) •
[🔗 LinkedIn](https://www.linkedin.com/in/eddierosas21) •
[💻 GitHub Profile](https://github.com/erosas9172)

---

## 🔍 Project Overview

This capstone project analyzes **San Francisco Police Department (SFPD) incident reports from 2020–2024** to understand how crime patterns change over time and space.

Using **Python, time-series modeling, and GIS**, the project:

- Explores **temporal trends** (hour, day-of-week, month, year)
- Visualizes **spatial patterns** across police districts and neighborhoods
- Builds **forecasting models** (Prophet & SARIMAX) for daily incident counts
- Trains a **Decision Tree classifier** using engineered temporal and socio-economic features
- Integrates outputs into an **ArcGIS Dashboard** and web-based project site

---

## 🗂 Repository Contents

- `index.html` – Main project website with tabs for Home, Dashboard, Models, SWOT, and About  
- `BDA600_Final_Project_Report.pdf` – Full written capstone report  
- `SF_Crime_Cycles.ipynb` – Core analysis notebook (EDA, modeling, and figures)
- `figures/` *(or PNGs in root, depending on structure)* – Visualization assets embedded in the site:
  - SARIMAX & Prophet forecasts and components
  - Decision Tree feature importance plots
- `data/` *(CSV / Parquet files)* – Processed datasets used in the analysis:
  - `sfdp_2020_2024_clean.parquet`
  - `sfdp_daily_features.parquet`
  - `district_counts_2020_2024.csv`
  - `predicted_hotspots.csv`
  - `prophet_forecast_30days.csv`
  - `sfdp_daily_features_sample.csv`

> **Note:** Raw data comes from the City and County of San Francisco open data portal:  
> https://data.sfgov.org/Public-Safety/Map-of-Police-Department-Incident-Reports-2018-to-/jq29-s5wp

---

## 🧠 Methods & Models

- **Time-Series Forecasting**
  - SARIMAX \((1,1,1)(1,1,1,7)\) with weekly seasonality
  - Facebook **Prophet** with daily observations and weekly/yearly components
  - Evaluated with MAE, RMSE, and MAPE on a 60-day holdout window

- **Classification**
  - Tuned **Decision Tree classifier** on daily features
  - Macro-F1 ≈ 0.61 and ROC-AUC ≈ 0.65
  - Top predictors: lagged incident counts, month, day-of-week, key incident categories

- **Visualization & GIS**
  - Python (pandas, matplotlib, seaborn, GeoPandas)
  - **ArcGIS Dashboard** for interactive spatial-temporal exploration
  - Web front-end built with HTML/CSS and embedded maps/figures

---

## 🚀 How to View the Project

1. Visit the live site:  
   **https://erosas9172.github.io/BDA600_Capstone/**
2. Explore:
   - **Home:** project context and overview
   - **Dashboard:** embedded ArcGIS Dashboard
   - **Machine Learning Models:** SARIMAX, Prophet, and Decision Tree results
   - **SWOT Analysis:** strengths, weaknesses, opportunities, and threats
   - **About:** team, course, and contact info

---

## 👤 About the Author

I’m **Eddie Rosas**, an M.S. Big Data Analytics student at San Diego State University with a background in
data analysis, banking operations, and geospatial analytics.

- LinkedIn: https://www.linkedin.com/in/eddierosas21  
- GitHub: https://github.com/erosas9172

