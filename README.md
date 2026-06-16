# 🌍 COVID-19 Global Data Analysis & Visualization

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific_Computing-013243?style=for-the-badge&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</p>

<p align="center">
  <b>End-to-End COVID-19 Data Analysis Project</b><br>
  Data Cleaning • Exploratory Data Analysis • Time Series Analysis • Data Visualization • Insight Generation
</p>

---

## 📌 Project Overview

This project analyzes global COVID-19 trends using confirmed cases, deaths, and recovery datasets.

The objective was to transform raw multi-sheet COVID-19 data into meaningful insights through:

- Data Cleaning & Preprocessing
- Data Transformation (Wide → Long Format)
- Exploratory Data Analysis (EDA)
- Time-Series Analysis
- Recovery & Fatality Analysis
- Country-Level Comparisons
- Advanced Visualizations
- Insight Generation

---

## 🚀 Key Features

✅ Cleaned and merged datasets from multiple sheets

✅ Converted cumulative reports into daily metrics

✅ Analyzed:

- Confirmed Cases
- Deaths
- Recoveries
- Recovery Rate
- Case Fatality Rate (CFR)

✅ Created professional visualizations

✅ Generated country-level and regional insights

✅ Produced a reusable cleaned dataset

---

## 🛠️ Tech Stack

| Tool | Usage |
|--------|--------|
| Python | Programming |
| Pandas | Data Cleaning & Analysis |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| OpenPyXL | Excel Processing |
| Jupyter Notebook | Development |

---

## 📂 Project Structure

```text
COVID19-Global-Data-Analysis
│
├── data/
│   ├── covid_19_dataset.xlsx
│   └── merged_clean.csv
│
├── images/
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
│   └── COVID19_Case_Study.ipynb
│
├── insights_summary.txt
├── requirements.txt
└── README.md
```

---

# 📊 Key Findings

## Top Countries by Confirmed Cases

| Country | Cases |
|----------|----------|
| USA | 33.3 Million |
| India | 27.9 Million |
| Brazil | 16.5 Million |

---

## Countries with Highest Average Daily Deaths

| Country | Avg Daily Deaths |
|----------|------------------|
| USA | 12,784 |
| Brazil | 10,175 |
| India | 5,974 |
| Mexico | 5,068 |
| United Kingdom | 2,847 |

---

## 📈 Visualizations

### Top 10 Countries by Confirmed Cases

![Top Countries](images/2b_top10_countries_confirmed.png)

---

### China COVID-19 Trend Analysis

![China Trend](images/2c_china_confirmed_trends.png)

---

### Peak Daily Cases Analysis

#### Germany • France • Italy

![Peak Cases](images/5a_peak_daily_confirmed_germany_france_italy.png)

---

### Recovery Rate Comparison

#### Canada vs Australia

![Recovery Rate](images/5b_recovery_rate_canada_australia.png)

---

### COVID-19 Death Distribution in Canada

![Canada Deaths](images/5c_canada_deaths_cfr.png)

---

### Top 5 Countries by Average Daily Deaths

![Top Deaths](images/6c_top5_avg_daily_deaths.png)

---

### United States Death Evolution

![USA Deaths](images/6d_us_deaths_evolution.png)

---

### Monthly Progression Analysis

#### USA • Italy • Brazil

![Monthly Progression](images/7b_monthly_progression_us_italy_brazil.png)

---

### Top Countries by Average Daily Deaths (2020)

![Top Deaths 2020](images/8a_top3_avg_daily_deaths_2020.png)

---

### South Africa Recovery Analysis

![South Africa Recovery](images/8b_south_africa_recoveries.png)

---

### USA Recovery Analysis

![USA Recovery](images/8c_us_monthly_recovery_ratio.png)

---

## 📋 Data Processing Workflow

```mermaid
flowchart LR

A[Raw Excel Data]
--> B[Data Cleaning]

B --> C[Wide to Long Conversion]

C --> D[Merge Datasets]

D --> E[Feature Engineering]

E --> F[EDA]

F --> G[Visualization]

G --> H[Insights & Conclusions]
```

---

## 📌 Challenges Solved

- Missing values handling
- Date normalization
- Multi-sheet integration
- Wide-to-long reshaping
- Daily metric calculations
- Recovery rate calculations
- Fatality rate calculations

---

## 📈 Future Improvements

- Interactive Power BI Dashboard
- Tableau Visualization
- Streamlit Web App
- Forecasting Models
- Per-Capita Analysis
- Vaccination Impact Study

---

## ▶️ Run Locally

Clone the repository

```bash
git clone https://github.com/mukherjeesourav687/COVID19-Global-Data-Analysis.git
```

Move into the project

```bash
cd COVID19-Global-Data-Analysis
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

---

## 👨‍💻 Author

### Sourav Mukherjee

Aspiring Data Analyst | Python Developer | Data Science Enthusiast

📧 Add your email

🔗 Add your LinkedIn

🔗 Add your GitHub

---

## ⭐ If you found this project useful

Please consider giving this repository a **Star ⭐**

It helps support the project and motivates future improvements.
