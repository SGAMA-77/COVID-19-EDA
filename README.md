# COVID-19 Exploaratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.2.0-%23015055)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.3.4-%23ffffff?logo=matplotlib)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11.1-%230C7BDC)

## Overview
This project performs an Exploratory Data Analysis on the COVID-19 dataset from Johns Hopkins University.
The goal is to uncover trends in confirmed cases, deaths and recoveries globally and the country level.
Key analyses include:
- Global infection trends over time
- Top 10 most affected countries
- Mortality and recovery rate calculations
- Correlation analysis between metrics

**Skills Demonstrated**: Data cleaning, time-series analysis, visulaization, feature engineering.

---

## Dataset
**Source**: [Johns Hopkins University GitHub Repository](https://github.com/CSSEGISandData/COVID-19)  
**Context**:  
- Daily-level data starting from 22 Jan 2020
- Tracks cumulative confirmed cases, deaths, and recoveries
- Originally collected by WHO and curated by Johns Hopkins

### Column Descriptions
| Column | Description |
|--------|-------------|
| `ObservationDate` | Date of observation (MM/DD/YYYY) |
| `Country/Region` | Country or region of observation |
| `Confirmed` | Cumulative confirmed cases |
| `Deaths` | Cumulative deaths |
| `Recovered` | Cumulative recoveries |

---

## Analysis Steps
1. **Data Cleaning**  
   - Handled missing values by filling with zeros
   - Converted `ObservationDate` to datetime format
   - Dropped irrelevant columns (`SNo`, `Last Update`)

2. **Global Trends**  
   - Time-series line plots for confirmed cases, deaths, and recoveries
   - Identified peak infection periods

3. **Country-Wise Analysis**  
   - Top 10 countries by confirmed cases (bar plots)
   - Mortality and recovery rate comparisons

4. **Advanced Insights**  
   - Heatmap showing correlations between metrics
   - Calculated mortality rate = `(Deaths / Confirmed) * 100`

---

## Key Insights
- **Global Case Growth**: Exponential rise in confirmed cases from March 2020 onward.
- **Country Disparities**: [Country X] had the highest mortality rate ([X]%), likely due to [hypothesis].
- **Recovery Correlation**: Strong positive correlation (+0.89) between confirmed cases and recoveries.

---

## Tools Used
- **Python Libraries**: Pandas, Matplotlib, Seaborn, NumPy
- **Data Sources**: Johns Hopkins CSSE COVID-19 Dataset
- **Visualization**: Line plots, bar charts, heatmaps

---

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/SGAMA-77/COVID-19-EDA.git
   