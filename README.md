# 🗳️ Advanced Geospatial Election Integrity Analysis - Anambra

This project provides a deep analytical and visual exploration of election data in Anambra State, Nigeria. Using advanced geospatial techniques, outlier detection algorithms, and contextual demographic analysis, it uncovers patterns in voter engagement, turnout irregularities, and potential anomalies from 1999 to 2023.

## 📌 Project Summary

The dashboard is divided into three interactive pages:

1. **Executive Overview** – High-level KPIs, trends in party votes, turnout patterns, demographics, and urban vs rural participation.
2. **Outlier Analysis** – Highlights clusters with unusual voting behavior using DBSCAN clustering.
3. **Cluster Tooltip Page** – Dynamic insight popups for each cluster, showing voting unit count and share of outliers.

---

## 📊 Key Features

### ✅ Page 1: Executive Overview
![image](https://github.com/user-attachments/assets/faa49b20-7ff3-432c-9f3d-0fd893844d70)

- **KPIs**: Total Registered Voters (10M), Total Accredited Voters (4M).
- **Party Vote Trends**: Interactive filters show APC & PDP performance over the years.
- **Turnout Over Time**: Bar + Line combo to show how voter turnout (%) compares with registration trends.
- **Urban vs Rural Population (2003–2019)**: Shows population shift that may influence voter behavior.
- **Demographic Influence**: Maps population distribution to voting participation.
- **Voter Engagement Correlation**: Plots accredited voters vs population to identify turnout consistency.

### 🧪 Page 2: Outlier Analysis
![image](https://github.com/user-attachments/assets/5d5cdb99-22dd-4bdd-8d0a-31f1b3d4c986)

- **DBSCAN Clustering (500m radius)** applied to geospatial voting units to detect voting anomalies.
- **Cluster with Most Outliers**: ID `286` has the highest flagged outliers.
- **Final Outlier Flag (True/False)**: Percentage of anomalous units shown on bar chart & map.
- **Voting Unit Anomaly Map**: Microsoft Bing base map used for spatial pattern display.
- **Turnout Treemap**: Quickly shows which years had lower or higher participation density.
- **Population vs Accredited Voters**: Emphasizes magnitude differences by outlier status.

### 🧩 Tooltip Page
- **Polling Units in Cluster**: Total units associated with each cluster ID.
- **Outlier Share (Gauge)**: Proportion of those units flagged as anomalies.

---

## 🧠 Insights & Findings

- **Cluster 286** contributed disproportionately to the total outliers.
- **Outlier Units** had significantly lower accredited voter counts compared to non-outliers.
- **2015** and **2003** stood out with higher turnout percentages, while **2023** had many flagged clusters.
- **Urbanization** increased steadily from 2003 to 2019, possibly impacting the voter turnout imbalance.
- **Registered voters** do not always correlate with turnout, highlighting discrepancies that require further auditing.

---

## 🛠️ Tools & Technologies

- **Power BI** for interactive dashboard design and visuals
- **Python** (used for preprocessing, clustering, DBSCAN labeling)
- **Pandas & Numpy** for data wrangling
- **Scikit-learn** for DBSCAN algorithm
- **Jupyter Notebook** for EDA and cluster validation
- **Power BI DAX** for KPI, measure calculations and dynamic tooltips

