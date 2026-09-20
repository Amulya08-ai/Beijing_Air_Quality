# Beijing Air Quality — Data Analysis

## 📌 Project Overview

This project analyzes the **Beijing Multi-Site Air Quality Dataset** to understand air pollution patterns across multiple monitoring stations in Beijing.

The analysis was performed using **Python, Pandas, NumPy, Matplotlib, Seaborn, and Plotly**.

The dataset contains hourly air-quality and weather measurements collected from **12 monitoring stations**.

---

## 🎯 Objectives

* Explore the structure and quality of the dataset
* Analyze major air pollutants
* Identify pollution trends over time
* Compare pollution levels across monitoring stations
* Study the relationship between weather conditions and pollution
* Detect missing and invalid values
* Identify potential outliers
* Prepare a clean dataset for further SQL, Machine Learning, and Deep Learning analysis

---

## 📊 Dataset

The dataset contains approximately **420,000 hourly observations** from 12 monitoring stations.

### Air Pollutants

* PM2.5
* PM10
* SO2
* NO2
* CO
* O3

### Weather Variables

* TEMP — Temperature
* PRES — Atmospheric Pressure
* DEWP — Dew Point
* RAIN — Rainfall
* wd — Wind Direction
* WSPM — Wind Speed

### Time Variables

* Year
* Month
* Day
* Hour

### Station

The dataset contains measurements from 12 monitoring stations:

* Aotizhongxin
* Changping
* Dingling
* Dongsi
* Guanyuan
* Gucheng
* Huairou
* Nongzhanguan
* Shunyi
* Tiantan
* Wanliu
* Wanshouxigong

---

## 🔍 Analysis Performed

### 1. Data Understanding

* Dataset shape
* Column information
* Data types
* Statistical summary
* Unique stations
* Time-period analysis

### 2. Data Quality Analysis

Checked for:

* Missing values
* Duplicate records
* Invalid numerical values
* Data-type inconsistencies
* Negative pollutant readings
* Potential outliers

### 3. Data Cleaning

The following preprocessing steps were performed:

* Converted numerical columns to appropriate numeric types
* Converted invalid negative pollutant/weather readings to missing values where appropriate
* Filled missing numerical values using station-wise median values
* Filled remaining missing values using overall medians
* Filled missing wind-direction values using the mode
* Created useful time-based features
* Sorted observations by station and time

> Temperature and dew-point values were not treated as invalid merely because they were negative, since negative values are physically possible for these variables.

---

## 📈 Exploratory Data Analysis

The analysis includes visualizations for:

* Pollutant distributions
* Pollution trends over time
* Monthly pollution patterns
* Hourly pollution patterns
* Day-of-week pollution patterns
* Station-wise pollution comparison
* Pollutant comparison
* Pollutant correlation
* Weather vs pollution relationships

Interactive visualizations were also created using **Plotly**.

---

## 🌫️ Overall Air Quality Analysis

An AQI-style analysis was created to understand overall air-quality trends across different time periods.

The analysis considers:

* PM2.5
* PM10
* NO2
* SO2
* CO
* O3

The AQI-style value is used for **analytical visualization and comparison**, rather than being presented as an official CPCB AQI calculation, because the dataset contains hourly observations and official AQI calculations depend on specified averaging periods.

---

## 🧹 Output

After cleaning and preprocessing, the final dataset was saved as:

```text
beijing_air_quality_cleaned.csv
```

This cleaned dataset is used as the input for the next stages of the project.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Google Colab
* GitHub

---

## 📁 Files

```text
01_Analysis/
│
├── Beijing_Air_Quality_Analysis.ipynb
└── README.md
```

---

## 🚀 Project Roadmap

This analysis is the first stage of a larger end-to-end data project.

```text
Python Data Analysis
        ↓
Streamlit Dashboard
        ↓
SQL Analysis
        ↓
Machine Learning
        ↓
Deep Learning
        ↓
Agentic AI
```

The cleaned dataset produced during this stage will be reused throughout the later stages of the project.

---

## 👩‍💻 Author

**Amulya**

Data Science & AI Learning Project
