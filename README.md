 machine-learning-covid-19-forcast-
 
 📌 Project Overview

This project analyzes the global and India-specific trends of the COVID-19 pandemic using Python. It includes interactive visualizations, rate analysis, and a 7-day ahead forecast using Facebook Prophet.

---

 🎯 Objectives

- Visualize the impact of COVID-19 (confirmed, deaths, recovered, active)
- Analyze the rate of infection and recovery over time
- Compare India vs Global trends
- Build a time-series forecasting model to predict cases 7 days into the future

---

 📁 Project Structure

```
COVID19-Analysis/
│
├── COVID19_Analysis.ipynb     ← Main Jupyter Notebook (all code here)
├── README.md                  ← This file
│
└── data/                      ← (Optional) Place your CSV/Excel files here
    ├── time_series_covid19_confirmed_global.csv
    ├── time_series_covid19_deaths_global.csv
    ├── time_series_covid19_recovered_global.csv
    └── covid_19_india.csv
```

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, and aggregation |
| `numpy` | Numerical operations |
| `plotly` | Interactive visualizations and charts |
| `prophet` | Facebook's time-series forecasting model |
| `requests` | Auto-fetching dataset from GitHub |
| `matplotlib` | Prophet component plots |

---

📦 Installation
Google Colab (Recommended, Zero Setup)
1. Open [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Upload Notebook**
3. Upload `COVID19_Analysis.ipynb`
4. Click **Runtime → Run All**
5. The first cell installs everything automatically ✅


 📊 Dataset

 Auto-Fetch (Default — No Download Needed)
The notebook automatically pulls live data from **Johns Hopkins CSSE** GitHub:
- ✅ `time_series_covid19_confirmed_global.csv`
- ✅ `time_series_covid19_deaths_global.csv`
- ✅ `time_series_covid19_recovered_global.csv`

 Manual Download Options

| Source | Link | Contents |
|--------|------|----------|
| Johns Hopkins CSSE | [GitHub Link](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series) | Global CSV files |
| Kaggle — India | [Dataset Link](https://www.kaggle.com/datasets/sudalairajkumar/covid19-in-india) | India state-wise data |
| Kaggle — Global | [Dataset Link](https://www.kaggle.com/datasets/imdevskp/corona-virus-report) | Global + country CSV/Excel |

---

 📓 Notebook Walkthrough

| Step | Section | Description |
|------|---------|-------------|
| 1 | Install & Import | Installs all libraries, imports them |
| 2 | Load Data | Auto-fetches JHU data (with offline fallback) |
| 3 | Global Trend | Cumulative confirmed, deaths, recovered, active |
| 4 | Daily New Cases | Bar chart with 7-day rolling average |
| 5 | India Dashboard | 4-panel: cumulative, daily, recovery rate, fatality rate |
| 6 | Top 10 Countries | Horizontal bar chart ranked by confirmed cases |
| 7 | World Map | Choropleth map of global confirmed cases |
| 8 | Prophet Model | Train Facebook Prophet on global confirmed cases |
| 9 | Forecast Chart | 7-day ahead forecast with 95% confidence band |
| 10 | Forecast Table | Predicted values with lower/upper bounds |
| 11 | Rate Comparison | Recovery % vs Fatality % for Global and India |

---

 📈 Sample Outputs

```
📋 7-Day COVID-19 Forecast (Global Confirmed Cases)

Date          Predicted Cases    Lower Bound    Upper Bound
----------    ---------------    -----------    -----------
2021-08-01    210,345,000        208,100,000    212,600,000
2021-08-02    210,890,000        208,500,000    213,200,000
...
```

---

 
