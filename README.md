# 📊 Customer Churn Analysis Dashboard

**Repository:** https://github.com/prasanna-882/Customer-Churn-Analysis

---

## 🚀 Project Overview

The **Customer Churn Analysis Dashboard** project focuses on analyzing large-scale customer data to identify churn patterns, high-risk customer segments, and key retention drivers. The goal is to enable data-driven decision-making by delivering actionable insights through exploratory analysis, automated reporting, and interactive dashboards.

The dataset (**4.4L+ records**) used in this project is sourced from **Kaggle** and was ingested into **MySQL** for reporting and analytical processing.

### Key Project Activities

- Collected, cleaned, and transformed **1.9L+** customer transaction records from MySQL for analytical reporting.
- Performed Exploratory Data Analysis (EDA) using Python to uncover churn drivers, behavioral trends, and customer risk segments.
- Designed and developed interactive Power BI dashboards to monitor churn trends, retention KPIs, cohort analysis, and customer segmentation.
- Built advanced DAX measures to calculate churn rate, customer lifetime value (CLV), retention percentage, and time-based metrics.
- Automated monthly churn reporting using Python scripts and SQL, reducing manual reporting efforts by approximately **25%**.
- Optimized data models and DAX calculations to improve dashboard performance and refresh efficiency.
- Delivered actionable insights to marketing and customer success teams, supporting effective retention strategies and business decisions.

---

## 🎯 Business Objective

Customer churn directly impacts revenue and organizational growth.  
**Objective:** Understand why customers leave (churn), identify patterns and segments at risk, and empower business teams with insights and automated reporting to improve retention strategies.

---

## 📁 Repository Structure
```
Customer-Churn-Analysis Dashboard/
│
├── Data/
│ ├── raw/
│ │ └── customer_churn_raw.csv
│ │
│ ├── processed/
│ │ └── customer_churn_cleaned.csv
│ │
│ └── data_dictionary/
│ └── data_dictionary.xlsx
│
├── SQL/
│ ├── schema/
│ │ └── create_tables.sql
│ │
│ ├── data_load/
│ │ └── load_data.sql
│ │
│ ├── eda_queries/
│ │ └── churn_analysis.sql
│ │
│ └── reporting_queries/
│ └── churn_kpis.sql
│
├── Python/
│ ├── notebooks/
│ │ ├── 01_data_cleaning.ipynb
│ │ ├── 02_eda.ipynb
│ │ ├── 03_churn_driver_analysis.ipynb
│ │ └── 04_feature_engineering.ipynb
│ │
│ ├── scripts/
│ │ └── monthly_churn_report.py
│ │
│ └── utils/
│ └── helper_functions.py
│
├── Power_BI/
│ ├── datasets/
│ │ └── churn_model.pbix
│ │
│ ├── dax_measures/
│ │ └── churn_dax_measures.txt
│ │
│ └── exports/
│ └── churn_dashboard_images/
│
├── Insights/
│ ├── key_findings.md
│ ├── churn_drivers.md
│ └── recommendations.md
│
├── Documentation/
│ ├── project_overview.md
│ ├── data_pipeline.md
│ ├── dashboard_design.md
│ └── business_impact.md
│
├── README.md

```


---

## 🧰 Tools & Technologies

| Category | Tools |
|----------|-------|
| Data Storage & SQL | MySQL |
| Analytics & Data Processing | Python (Pandas, NumPy, Matplotlib, Seaborn) |
| Dashboard & Reporting | Power BI (DAX, Data Modeling) ||
| Documentation | Excel, Markdown |

---

## 📊 Data Pipeline

### 🔹 Data Source
Raw customer churn data was provided in CSV format from Kaggle and stored in the `Data/raw` directory.

### 🔹 Processing Steps
- Raw data was ingested and stored in MySQL.
- Data cleaning & preprocessing using Python:
  - Handling data types & missing values
  - Validating churn values
- Cleaned data saved in `Data/processed`

---

## 🧠 Analytics & Reporting

### 🔹 SQL Layer
- Database tables created using SQL schema scripts.
- Data loaded and transformed for analysis and KPI reporting.
- SQL queries designed for churn metrics and segment analysis.

### 🔹 Python Analysis
- Used Python for exploratory data analysis (EDA).
- Identified churn drivers and risk factors.
- Performed feature engineering for churn insights.

### 🔹 Power BI Dashboard
- Developed interactive dashboard with multiple report pages.
- Built advanced DAX measures to compute churn rate, retention, CLV, and risk metrics.
- Optimized model performance and refresh efficiency.

---

## 📈 Dashboard Design

Power_BI/exports/churn_dashboard_images/home.png

### 🗂 Pages Overview
- **Home** — Overview and navigation
<img width="1390" height="779" alt="Home" src="https://github.com/user-attachments/assets/26afdddf-5150-4ee6-b17b-f9d4293444a9" />
  
- **Executive Summary** — Top-level KPIs
<img width="1386" height="777" alt="Executive Overview" src="https://github.com/user-attachments/assets/9115558b-a358-4cdf-b1bb-81854a3fc813" />
  
- **Churn Trends** — Time-series analysis
<img width="1387" height="781" alt="Churn Trends" src="https://github.com/user-attachments/assets/15ac1a18-76b7-4ccc-ac03-442fda560f1b" />
  
- **Customer Segmentation** — Risk & behavior segments
<img width="1388" height="782" alt="Cust Segmentation" src="https://github.com/user-attachments/assets/67109adb-a9eb-4f67-9b26-15f1e1add145" />
  
- **Churn Drivers** — Behavioral drivers and patterns
<img width="1388" height="783" alt="Churn Drivers" src="https://github.com/user-attachments/assets/31410542-862d-4068-b33a-422f21d4f567" />
  
- **Insights & Recommendations** — Business-focused takeaways
<img width="1391" height="781" alt="Insights   Recommendation" src="https://github.com/user-attachments/assets/006a836f-1713-45ae-85eb-901b07618dac" />


### 🎨 Design Principles
- Interactive filter-based navigation  
- KPI-first layout for business decision-making  
- Consistent visual encoding and color use  

---

## 💡 Key Findings

### 🔍 Overall Insights
- Churn remains a significant challenge with varied patterns across segments.
- Customers on premium plans show better retention.

### 📊 Behavior Insights
- High support calls indicate dissatisfaction & increase churn risk.
- Late payments strongly correlate with churn behavior.
- Low platform usage results in early churn.

### ⚠️ Risk Groups
High-risk customers were identified using combined risk factors:

- Support Calls ≥ 5  
- Payment Delays ≥ 15 days  
- Usage Frequency ≤ 5  

---

## 🧩 Churn Drivers

- **High Support Dependency** — Poor customer satisfaction.  
- **Frequent Payment Delays** — Weak purchase commitment.  
- **Low Usage Frequency** — Weak engagement and product value.  
- **Subscription Type Impact** — Basic-tier churn higher than premium.  
- **Combined Risk Impact** — Several risk factors increase churn probability.  

---

## 📊 DAX Measures (Highlights)

Here are a few key DAX measures from the project:

### 🔹 Total Customers
```dax
Total Customers = CALCULATE(DISTINCTCOUNT('Customer Churn'[customer_id]), REMOVEFILTERS('Customer Churn'[churn]))
```

🔹 Churn Rate
```dax
Churn Rate = DIVIDE([Churned Customers], [Total Customers])
```

🔹 Retention Rate
```dax
Retention Rate = 1 - [Churn Rate]
```

🔹 High-Risk Customers
```dax
High Risk Customers =
CALCULATE(
    DISTINCTCOUNT('Customer Churn'[customer_id]),
    'Customer Churn'[support_calls] >= 5,
    'Customer Churn'[payment_delay] >= 15,
    'Customer Churn'[usage_frequency] <= 5
)
```
---- 

## ⚙️ Automation  

- Monthly churn reporting automated using Python.

- Execution scheduled via Windows Task Scheduler.

- Reduced manual reporting time by ~25%.

--- 

---

## 🧠 Business Impact
1. 📉 Operational

- Consistent automated reporting

- Reduced manual efforts & errors

2. 📊 Strategic

- Improved retention strategies

- Identified priority customer segments

- Helps maximize Customer Lifetime Value (CLV)

--- 

## 📈 Future Enhancements

✔ Build Predictive Machine Learning churn model  
✔ Real-time dashboard refresh via streaming data  
✔ Alerting system for high-risk customer events  
✔ Deploy dashboard to Power BI Service  

--- 

## 🙏 Acknowledgement

Special thanks to the **Kaggle Customer Churn Dataset** for providing an excellent real-world dataset.  
This project was created as part of a **Data Analytics learning journey** using **Power BI, Python, and SQL**.

---

## 📎 Author

**👤 Name:** Prasanna   
**💻 GitHub:** [prasanna-882](https://github.com/prasanna-882)  


---


