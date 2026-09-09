# ✈️ Automated Flight Booking & Pricing BI Pipeline

An end-to-end Data Engineering and Business Intelligence project simulating a travel-tech analytics pipeline. This project extracts, transforms, and loads (~300,000 records) of flight data into an optimized MySQL Star Schema, visualized via an interactive Tableau dashboard to derive pricing and route insights.

## 📊 Project Architecture
1. **Extract & Transform:** Python (Pandas) for data cleaning, handling missing values, and structuring data into Fact and Dimension tables.
2. **Load (Data Warehouse):** Loaded into MySQL (via Laragon) establishing a relational Star Schema.
3. **Visualization:** Tableau Public 4-quadrant interactive dashboard for business insights.

## 🛠️ Tech Stack
* **Programming Language:** Python (Pandas, SQLAlchemy, PyMySQL)
* **Database:** MySQL / phpMyAdmin (Laragon)
* **BI Tool:** Tableau Public
* **Version Control:** Git & GitHub

## 📂 Dataset Source
The raw data used for this project is sourced from Kaggle:
* [Airlines Flights Dataset by Rohit Grewal](https://www.kaggle.com/datasets/rohitgrewal/airlines-flights-data)

## 🚀 Key Business Insights
* **Premium Carriers:** Vistara and Air India exhibit the highest average ticket prices.
* **Class Disparity:** Business class tickets average ~8x higher prices than Economy class.
* **Route Density:** Delhi-Mumbai serves as the core high-volume traffic corridor.
* **Dynamic Pricing:** Ticket prices fluctuate significantly based on proximity to the departure date (`days_left`).

## 📁 Repository Structure
```text
├── 1_etl_pipeline.ipynb       # Python script for ETL and Star Schema creation
├── tableau/                   # Tableau workbook files (.twb)
├── .gitignore                 # Excludes local CSV datasets and temp files
└── README.md                  # Project documentation