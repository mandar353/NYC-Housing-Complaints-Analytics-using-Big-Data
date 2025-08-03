# 🏙️ NYC Housing Complaints Analytics using Big Data

---

## ✅ Problem Statement
Analyzing large-scale NYC housing complaint data to uncover trends, resolution delays, and neighborhood-wise complaint patterns using distributed processing with PySpark.

---

## 🎯 Project Objectives
- 🏘️ Identify complaint-prone areas and buildings  
- 📊 Design an **Affordable Living Index (ALI)**  
- 🔄 Integrate multiple housing datasets into a unified **data lake**  
- 📉 Visualize insights through **interactive dashboards**  
- 🧠 Support **data-driven decisions** for authorities and tenants  

---

## 🗂️ Data Sources

| Dataset               | Source                                                                 | Purpose              |
|-----------------------|------------------------------------------------------------------------|----------------------|
| 311 Service Requests  | [Link](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9) | Complaint prediction |
| HPD Maintenance Issues| [Link](https://data.cityofnewyork.us/Housing-Development/Housing-Maintenance-Code-Complaints-and-Problems/ygpa-z7cr) | Issue validation     |
| PLUTO Land Use        | [Link](https://data.cityofnewyork.us/City-Government/Primary-Land-Use-Tax-Lot-Output-PLUTO-/64uk-42ks) | Building metadata    |

---

## ⚙️ Project Architecture

📂 S3 (Raw Data)  
       ↓  
🧭 AWS Glue  (Crawlers, ETL)  
       ↓  
🔥 Apache Spark on EMR  (Data Cleaning, Joins, Aggregation)  
       ↓  
📂 S3 (Processed Data)  
       ↓  
🔍 Amazon Athena  (SQL Queries)  
       ↓  
📊 Power BI  (Dashboard Visualization)

---

## 💻 Tools & Technologies
- **AWS S3** – Data lake storage (raw + cleaned)
- **AWS Glue** – ETL and schema catalog
- **Apache Spark (PySpark)** – Distributed processing on EMR
- **Parquet Format** – Efficient columnar storage
- **Databricks / Jupyter** – Code development & EDA
- **Power BI** – Dashboard & KPI visualization
- **Git / GitHub** – Version control

---

## 📍 Final Output
- **S3 Bucket:** `master-table-final`  
- **Folder:** `master_cleaned_data`  
- **File Format:** Parquet (.snappy)

---

## 📊 Sample Insights (Visualized using Power BI)

- ⏱️ **Average Resolution Time** per borough  
- 📈 **Top Complaint Types** by frequency  
- ❌ **Unresolved Complaints** trend over time  
- 🗺️ **Heatmap** of complaints (based on Latitude/Longitude)

---


