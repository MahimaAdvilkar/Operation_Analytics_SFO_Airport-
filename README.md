# Re-execute after kernel reset to regenerate the README file

# Create a polished README.md for the SFO Operations Analytics Project
sfo_readme = """
# ✈️ Passenger Flow and Operations at SFO – Operational Analytics Project

**Created by:** Mahima Advilkar  
**Role:** Data Analyst  
**Domain:** Operations Analytics | Aviation Industry  
**Tools Used:** Python, Excel, Tableau, Time Series Forecasting, Regression

---

## 📌 Project Overview

This project explores operational and passenger flow data at **San Francisco International Airport (SFO)**. By integrating two public datasets—Air Traffic Passenger Statistics and Landing Statistics—we applied regression and forecasting techniques to understand key trends, inform strategic airport planning, and enhance passenger experience.

---

## 🎯 Objectives

- Analyze what factors impact passenger flow the most  
- Forecast future passenger volumes using time series models  
- Identify operational bottlenecks across terminals and boarding areas  
- Derive actionable business recommendations for airport authorities

---

## 🧾 Datasets Used

- **Air Traffic Passenger Statistics**  
  Monthly passenger counts by terminal, boarding area, and activity type (deplaned, enplaned, transit)

- **Air Traffic Landings Statistics**  
  Landing information by aircraft type, weight, airline operations

📍 Source: [San Francisco Open Data Portal](https://data.sfgov.org)

---

## 🛠 Tools & Techniques

- Python, Pandas, Excel – Data integration, cleaning, analysis  
- Time Series Models – 3-Month Moving Average, Exponential Smoothing  
- Regression – Identify impact of aircraft and landing stats on flow  
- Tableau – Interactive dashboards for insights and presentation

---

## 📊 Key Insights

| Insight Category         | Observation |
|--------------------------|-------------|
| Passenger Variability    | Highest traffic in June 2024 (5,987); lowest in Nov 2023 (4,536) |
| Forecasting Accuracy     | Exponential Smoothing MAPE: 5.20% vs Moving Avg: 29.52% |
| Airline Ops              | United, SkyWest, Delta dominate operations |
| Aircraft Types           | Narrow-body aircraft dominate domestic routes |
| Boarding Areas           | Area A = 24,723 passengers; Area E = 2,929 (low traffic) |
| Regional Distribution    | Domestic: 54%, Asia: 22%, Europe: 14% |
| Annual Growth            | 345% traffic increase from 2023 to 2024 |

---

## 📈 Forecasting

| Month (2024) | Moving Avg Forecast | Exp. Smoothing Forecast |
|--------------|---------------------|--------------------------|
| October      | 5,437               | 5,360                    |
| November     | 5,411               | 5,072                    |
| December     | 5,321               | 5,214                    |

📉 **Exponential Smoothing** provided more accurate and stable predictions for future planning.

---

## 💡 Business Recommendations

- **Terminal Optimization**: Reallocate resources from Terminal 3 & 2 to high-traffic Terminal 1  
- **Expand International Routes**: Add flights to underserved regions (Middle East, Oceania)  
- **Develop Transit Hubs**: Improve services in transit-heavy regions like the US and Europe  
- **Optimize Boarding Areas**: Expand Area A, streamline low-traffic zones  
- **Cargo & Aircraft Ops**: Support freighter growth, invest in wide-body infrastructure  
- **Peak Readiness**: Use forecasts for seasonal staff and gate planning

---

## 📁 Repository Structure

| File                          | Description |
|-------------------------------|-------------|
| `SFO_Operations_Analysis.ipynb` | Data analysis & forecasting notebook |
| `passenger_landing_data.csv`   | Cleaned and merged dataset |
| `SFO_Passenger_Report.pdf`     | Final written report |
| `/visuals/`                    | Visual charts and graphs |
| `README.md`                    | Project documentation |

---

## 🔗 Tableau Dashboard

*Insert your Tableau Public link here if applicable*

---

> ⭐ If this project inspired you, feel free to star, fork, or connect!
"""

# Save the README to a file
readme_path = "/mnt/data/README_SFO_Operations.md"
with open(readme_path, "w") as f:
    f.write(sfo_readme)

readme_path
