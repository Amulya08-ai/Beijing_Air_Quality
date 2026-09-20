# 🌫️ Beijing Air Quality Analysis & Dashboard

## 📌 Project Overview

This project analyzes the **Beijing Multi-Site Air Quality Dataset** to understand air pollution patterns across Beijing.

The project uses **Python for data analysis and cleaning**, followed by an interactive **Streamlit dashboard** and **MySQL database setup** for structured data analysis.

The same cleaned dataset is being used throughout the project to maintain a consistent end-to-end workflow.

---

## 📊 Dataset

The dataset contains approximately **420,000 hourly observations** collected from **12 monitoring stations** in Beijing between **2013 and 2017**.

### Air Pollutants

* PM2.5
* PM10
* SO2
* NO2
* CO
* O3

### Weather Variables

* Temperature
* Atmospheric Pressure
* Dew Point
* Rainfall
* Wind Direction
* Wind Speed

### Monitoring Stations

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

# 🔍 1. Python Data Analysis

The dataset was explored and prepared using Python.

### Data Analysis

* Dataset shape and structure
* Data types
* Statistical summaries
* Missing-value analysis
* Duplicate checking
* Station-wise analysis
* Pollutant analysis
* Weather analysis
* Time-based analysis

### Data Cleaning

The following preprocessing was performed:

* Converted numerical columns to appropriate data types
* Checked pollutant values for invalid negative readings
* Preserved valid negative temperature and dew-point values
* Handled missing numerical values using median imputation
* Used station-wise medians where appropriate
* Handled missing wind-direction values using the mode
* Created useful time-based features
* Sorted records by station and time

### Exploratory Data Analysis

Visualizations were created to analyze:

* Pollutant distributions
* Pollution trends
* Monthly pollution patterns
* Hourly pollution patterns
* Day-of-week patterns
* Station-wise pollution levels
* Pollutant comparisons
* Pollutant correlations
* Weather vs pollution relationships

An **AQI-style trend** was also created to visualize overall air-quality patterns across different time periods.

> The AQI-style calculation is intended for analytical comparison and visualization and is not presented as an official CPCB AQI calculation.

### Technologies

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Plotly`

---

# 📊 2. Streamlit Dashboard

The cleaned dataset was used to build an interactive Streamlit dashboard.

### Dashboard Features

* Station selection
* Pollutant selection
* Year filtering
* Average, minimum and maximum pollutant values
* Record count
* Pollution trends
* Hourly pollution patterns
* Monthly trends
* Day-of-week analysis
* Station comparison
* Pollutant comparison
* Weather vs pollution analysis
* Pollutant correlation
* Overall air-quality trend
* Interactive Plotly charts

The dashboard allows users to explore pollution patterns interactively without directly modifying the analysis code.

### Technologies

`Python` · `Streamlit` · `Pandas` · `NumPy` · `Plotly`

---

# 🗄️ 3. MySQL Database Setup

The cleaned dataset is currently being prepared for SQL-based analysis using MySQL.

A relational database structure has been created with:

### `stations`

Stores the 12 monitoring stations.

### `air_quality`

Stores:

* Date/time components
* PM2.5
* PM10
* SO2
* NO2
* CO
* O3

### `weather`

Stores:

* Temperature
* Pressure
* Dew Point
* Rainfall
* Wind Direction
* Wind Speed

### `air_quality_raw`

A staging table matching the cleaned CSV structure is being used to load the data before inserting it into the normalized tables.

The database uses **Primary Keys and Foreign Keys** to establish relationships between the tables.

---

# 📁 Repository Structure

```text
Beijing_Air_Quality/
│
├── 01_Analysis/
│   ├── Beijing_Air_Quality_Analysis.ipynb
│   └── README.md
│
├── 02_Dashboard/
│   ├── Beijing_Air_Quality_Dashboard.py
│   └── README.md
│
├──  beijing_air_quality_cleaned.csv
│ 
│
└── README.md
```

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Streamlit
* MySQL
* SQL
* Google Colab
* GitHub

---

## 👩‍💻 Author

**Amulya**

Data Science & AI Learning Project
