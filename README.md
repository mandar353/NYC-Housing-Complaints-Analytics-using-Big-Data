✅ Project Title
NYC Housing Complaints Analytics using Big Data

✅ Problem Statement
Analyzing large-scale NYC housing complaint data to uncover trends, resolution delays, and neighborhood-wise complaint patterns using distributed processing with PySpark.

🎯 Project Objectives
•	Identify complaint-prone areas and buildings
•	Design an Affordable Living Index (ALI)
•	Integrate multiple housing datasets into a data lake
•	Visualize insights through interactive dashboards
•	Support data-driven decisions for authorities and tenants

🗂️ Data Source
Dataset	Description	Size/Volume	Key Columns
311 Service Requests (erm2-nwe9)
NYC citizen service complaints from 2010 onward	40.5 million rows, 41 columns	Unique Key, Created Date, Complaint Type, Borough, Status, Latitude, Longitude
Housing Maintenance Code Complaints (ygpa-z7cr)
Official housing code violation complaints	15.5 million rows, 33 columns	Complaint ID, Received Date, Problem Description, Status, Borough, Building ID
PLUTO (Primary Land Use Tax Lot Output)
NYC tax lot data with land use/zoning	850,000+ records, 101 columns	BBL, Land Use, Year Built, Lot Area, Units, Building Class

⚙️ Architecture Flow-
S3 (Raw Data)
↓
AWS Glue (Crawlers, ETL)
↓
Spark on EMR (Data Cleaning, Joins, Aggregation)
↓
S3 (Processed Data)
↓
Athena SQL Queries
↓
Power BI (Dashboards)

⚙️ Tools & Technologies
•	AWS S3 – Storage for source and target data
•	AWS Glue – Metadata Catalog & ETL
•	Apache Spark (PySpark) – Distributed data processing
•	Databricks / Jupyter – Development & notebooks
•	Parquet – Columnar data format
•	Git/GitHub – Version control

✅ Final Output Location
S3 Bucket: master-table-final
Folder: master_cleaned_data
Format: Parquet (.snappy)

📊 Sample Insights and KPI ( show in Power BI)
•	Average resolution time per borough.
•	Top complaint types by count.
•	Unresolved complaints trend over time.
•	Heatmap based on Latitude/Longitude.


