# Beijing Air Quality — Streamlit Dashboard

## 📌 Project Overview

This project includes an interactive **Streamlit dashboard** for exploring air-quality and weather data collected from 12 monitoring stations across Beijing.

The dashboard converts the results of the Python analysis into an interactive web application where users can filter the data and explore pollution patterns visually.

---

## 🎯 Dashboard Objectives

The dashboard allows users to:

* Explore air-quality measurements interactively
* Select different monitoring stations
* Select individual pollutants
* Filter data by year
* Compare pollution levels across stations
* Analyze pollution trends over time
* Understand hourly and monthly pollution patterns
* Explore relationships between weather and pollution
* Examine overall air-quality trends

---

## 🖥️ Dashboard Features

### 🔎 Interactive Filters

Users can filter the dashboard by:

* Monitoring station
* Pollutant
* Year

The charts and statistics update based on the selected filters.

---

### 📊 Key Performance Indicators

The dashboard displays:

* Average pollutant concentration
* Minimum value
* Maximum value
* Number of records

---

### 📈 Pollution Trend

Shows how the selected pollutant changes over time.

This helps identify periods of increasing or decreasing pollution.

---

### 🕐 Hourly Pattern

Displays pollution levels across different hours of the day.

This can help identify daily pollution patterns.

---

### 📅 Monthly Trend

Shows the selected pollutant's average level across months.

This helps identify seasonal patterns in air pollution.

---

### 📆 Day-of-Week Pattern

Compares pollution levels across different days of the week.

---

### 🏙️ Station Comparison

Compares pollution levels across Beijing's monitoring stations.

This helps identify geographical differences in pollution levels.

---

### 🌫️ Pollutant Comparison

Allows comparison of the major pollutants present in the dataset:

* PM2.5
* PM10
* SO2
* NO2
* CO
* O3

---

### 🌦️ Weather vs Pollution

The dashboard explores relationships between pollution and weather variables such as:

* Temperature
* Wind Speed

This helps investigate how weather conditions may be associated with pollutant concentrations.

---

### 🔗 Pollutant Correlation

A correlation analysis is provided to examine relationships between different pollutants.

---

### 🌫️ Overall Air Quality Trend

The dashboard provides an **AQI-style trend** using the major pollutants:

* PM2.5
* PM10
* NO2
* SO2
* CO
* O3

The visualization can show:

* Yearly overall air-quality trends when all years are selected
* Monthly trends when a specific year is selected
* Average AQI-style value
* Highest AQI-style value
* Dominant pollutant
* Period with the highest value

> The AQI-style calculation is intended for analytical visualization and comparison. It should not be interpreted as an official CPCB AQI because the dataset contains hourly observations and official AQI calculations use specified averaging periods.

---

## 🛠️ Technologies Used

* Python
* Streamlit
* Pandas
* NumPy
* Plotly

---

## 📂 Project Files

```text
02_Dashboard/
│
├── app.py
└── README.md
```

The `app.py` file contains the Streamlit application.

The dashboard uses:

```text
beijing_air_quality_cleaned.csv
```

as its data source.

---

## ▶️ Running the Dashboard

Install the required libraries:

```bash
pip install streamlit pandas numpy plotly
```

Run the application:

```bash
streamlit run app.py
```

The dashboard will open in the browser.

---

## 📌 Data Source

The dashboard is based on the **Beijing Multi-Site Air Quality Dataset**, containing hourly observations from 12 monitoring stations.

The data was cleaned and prepared during the Python analysis stage before being used by the dashboard.

---



The same cleaned dataset will be reused in the upcoming SQL and machine-learning stages.

---

## 👩‍💻 Author

**Amulya**

Data Science & AI Learning Project
