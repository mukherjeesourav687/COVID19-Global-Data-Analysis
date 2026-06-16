# COVID-19 Global Data Analysis & Visualization

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat-square&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-brightgreen?style=flat-square"/>
</p>

<p align="center">
  <a href="https://github.com/mukherjeesourav687/COVID19-Global-Data-Analysis">
    <img src="https://img.shields.io/badge/View%20on-GitHub-181717?style=flat-square&logo=github"/>
  </a>
  <a href="https://www.linkedin.com/in/mukherjeesourav687/">
    <img src="https://img.shields.io/badge/Connect-LinkedIn-0A66C2?style=flat-square&logo=linkedin"/>
  </a>
</p>

<p align="center">
  <strong>End-to-end analysis of global COVID-19 trends across 180+ countries</strong><br/>
  Data Cleaning · EDA · Time-Series Analysis · Recovery & Fatality Metrics · Visualization
</p>

---

## Overview

This project transforms raw, multi-sheet COVID-19 data into structured analytical insights — covering confirmed cases, deaths, and recoveries across countries from 2020 to 2021.

The focus is on solving real analytical problems: messy date formats, wide-format data that needs reshaping, multi-dataset merging, and deriving meaningful metrics like Case Fatality Rate (CFR) and Recovery Rate.

---

## Problem Statement

Raw COVID-19 datasets arrive fragmented across multiple sheets, in wide format, with inconsistent date columns, missing values, and no derived metrics. This project addresses:

- How do confirmed cases, deaths, and recoveries trend over time globally?
- Which countries had the highest fatality and recovery rates?
- How did the pandemic evolve month-over-month in key countries?
- What patterns emerge from daily vs cumulative metrics?

---

## Key Findings

| Metric | Value |
|---|---|
| Top country by confirmed cases | USA — 33.3 Million |
| 2nd highest confirmed cases | India — 27.9 Million |
| Highest average daily deaths | USA — 12,784/day |
| Highest recovery rate observed | Australia (vs Canada comparison) |
| Dataset coverage | 180+ countries, 2020–2021 |

### Countries by Average Daily Deaths

| Rank | Country | Avg Daily Deaths |
|---|---|---|
| 1 | USA | 12,784 |
| 2 | Brazil | 10,175 |
| 3 | India | 5,974 |
| 4 | Mexico | 5,068 |
| 5 | United Kingdom | 2,847 |

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core language |
| Pandas | Data manipulation, merging, reshaping |
| NumPy | Numerical computations |
| Matplotlib | Visualizations |
| OpenPyXL | Excel (.xlsx) file processing |
| Jupyter Notebook | Interactive analysis environment |

---

## Project Structure

```
COVID19-Global-Data-Analysis/
│
├── data/
│   ├── covid_19_dataset.xlsx       # Raw source data
│   └── merged_clean.csv            # Final cleaned & merged dataset
│
├── images/                         # All exported visualizations
│   ├── 2b_top10_countries_confirmed.png
│   ├── 2c_china_confirmed_trends.png
│   ├── 5a_peak_daily_confirmed_germany_france_italy.png
│   ├── 5b_recovery_rate_canada_australia.png
│   ├── 5c_canada_deaths_cfr.png
│   ├── 6c_top5_avg_daily_deaths.png
│   ├── 6d_us_deaths_evolution.png
│   ├── 7b_monthly_progression_us_italy_brazil.png
│   ├── 8a_top3_avg_daily_deaths_2020.png
│   ├── 8b_south_africa_recoveries.png
│   └── 8c_us_monthly_recovery_ratio.png
│
├── notebooks/
│   └── COVID19_Case_Study.ipynb    # Full analysis notebook
│
├── insights_summary.txt            # Written summary of findings
├── requirements.txt
└── README.md
```

---

## Data Processing Workflow

```
Raw Excel Data  →  Data Cleaning  →  Wide-to-Long Transform
      →  Dataset Merging  →  Feature Engineering
      →  EDA & Time-Series  →  Visualization  →  Insights
```

### Steps in detail

**1. Data Cleaning**
- Removed nulls and standardized inconsistent country names
- Normalized date columns across all three sheets

**2. Data Transformation**
- Reshaped wide-format date columns into long format using `pd.melt()`
- Calculated daily new cases from cumulative figures using `.diff()`

**3. Dataset Merging**
- Merged confirmed, deaths, and recovery DataFrames on `country` + `date`
- Exported unified dataset as `merged_clean.csv`

**4. Feature Engineering**
- Recovery Rate = Recovered / Confirmed × 100
- Case Fatality Rate (CFR) = Deaths / Confirmed × 100
- Monthly aggregations for trend analysis

**5. EDA & Visualization**
- Country-level comparisons, time-series trends, peak detection
- Rolling averages for smoothing daily fluctuation

---

## Visualizations

### Top 10 Countries by Confirmed Cases
![Top Countries](images/2b_top10_countries_confirmed.png)

### China — Confirmed Case Trend
![China Trend](images/2c_china_confirmed_trends.png)

### Peak Daily Cases — Germany, France, Italy
![Peak Cases](images/5a_peak_daily_confirmed_germany_france_italy.png)

### Recovery Rate — Canada vs Australia
![Recovery Rate](images/5b_recovery_rate_canada_australia.png)

### Case Fatality Analysis — Canada
![Canada CFR](images/5c_canada_deaths_cfr.png)

### Top 5 Countries by Average Daily Deaths
![Top Deaths](images/6c_top5_avg_daily_deaths.png)

### US Death Evolution Over Time
![US Deaths](images/6d_us_deaths_evolution.png)

### Monthly Progression — USA, Italy, Brazil
![Monthly](images/7b_monthly_progression_us_italy_brazil.png)

### Top 3 Countries by Avg Daily Deaths (2020)
![2020 Deaths](images/8a_top3_avg_daily_deaths_2020.png)

### South Africa — Recovery Trend
![SA Recovery](images/8b_south_africa_recoveries.png)

### USA — Monthly Recovery Ratio
![USA Recovery](images/8c_us_monthly_recovery_ratio.png)

---

## Challenges Solved

| Challenge | Approach |
|---|---|
| Wide-format date columns | `pd.melt()` to reshape into long format |
| Cumulative → daily metrics | `.diff()` per country group |
| Multi-sheet data integration | Sheet-wise read + merge on common keys |
| Missing values mid-series | Forward fill within country groups |
| Date normalization | `pd.to_datetime()` with format inference |
| Recovery & fatality rates | Derived columns via vectorized operations |

---

## Run Locally

```bash
# clone the repo
git clone https://github.com/mukherjeesourav687/COVID19-Global-Data-Analysis.git
cd COVID19-Global-Data-Analysis

# install dependencies
pip install -r requirements.txt

# launch notebook
jupyter notebook
```

Open `notebooks/COVID19_Case_Study.ipynb` and run cells in order.

---

## Future Scope

- [ ] Interactive Power BI / Tableau dashboard
- [ ] Streamlit web application for live exploration
- [ ] Per-capita analysis for fair country comparisons
- [ ] Vaccination impact analysis
- [ ] Geospatial choropleth maps
- [ ] Forecasting using ARIMA / Prophet

---

## Author

**Sourav Mukherjee**
Data Analyst · Python · SQL · Power BI

- GitHub: [github.com/mukherjeesourav687](https://github.com/mukherjeesourav687)
- LinkedIn: [linkedin.com/in/mukherjeesourav687](https://www.linkedin.com/in/mukherjeesourav687/)
- Email: mukherjeesourav687@gmail.com

---

*If this project helped you, consider giving it a ⭐ — it keeps the work going.*
