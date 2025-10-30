BDA600 Capstone: San Francisco Police Incident Analysis (2020–2024)
Overview

This repository contains the data and analysis for my BDA600 Capstone Project, part of the M.S. in Big Data Analytics program at San Diego State University.
The project explores patterns and trends in San Francisco Police Department (SFPD) incident reports from 2020 to 2024, using data analytics and machine learning techniques to identify spatial, temporal, and categorical patterns in crime distribution.

Project Objectives

Analyze temporal trends — Explore how incidents vary by hour, day, month, and year.

Investigate spatial distribution — Map and cluster crime locations by neighborhood and police district.

Categorize incidents — Identify which incident types and categories are most common.

Build predictive insights — Use machine learning to model or forecast incident patterns.



Dataset Information

File: sfpd_2020_2024_clean.parquet
Records: ~611,000 incidents
Columns: 14 fields

Incident Category, Incident Subcategory, Incident Date, Incident Time,
Latitude, Longitude, Police District, Analysis Neighborhood,
plus derived time features (hour, dayofweek, month, year).

Source: Public SFPD incident data portal
Preprocessing:

Removed duplicates and missing coordinates

Converted date/time fields

Engineered temporal features






Analytical Workflow

Data Cleaning & Transformation — Using pandas and NumPy.

Exploratory Data Analysis (EDA) — Descriptive stats, missing data, temporal and spatial visualizations.

Feature Engineering — Extracted hour, day, month, and year; handled geographic data.

Visualization — Heatmaps, time series plots, and spatial maps (Seaborn, Matplotlib, or Folium).

Modeling  — Predictive modeling or clustering of incidents.








Tools & Technologies
Category	Tools
Language	Python 3
Libraries	pandas, numpy, matplotlib, seaborn, geopandas, scikit-learn
Visualization	Folium, Plotly, Tableau, ArcGIS
Data Format	Parquet (efficient storage for large data)
Version Control	Git & GitHub
