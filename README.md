# azure-databricks-data-engineering-project
End-to-end Data Engineering project using Azure ADLS Gen2, Databricks, and PySpark
# Azure Data Engineering Project (Databricks + ADLS Gen2)

## 📌 Project Overview
This project demonstrates an end-to-end **Data Engineering pipeline** built using
**Azure Data Lake Storage Gen2** and **Azure Databricks** following the
**Medallion Architecture (Bronze → Silver → Gold)**.

## 🏗 Architecture
- Bronze Layer: Raw data ingestion
- Silver Layer: Cleaned & transformed data
- Gold Layer: Curated, analytics-ready datasets

## 🛠 Tech Stack
- Azure Data Lake Storage Gen2
- Azure Databricks
- PySpark
- Spark SQL
- OAuth (Service Principal authentication)

## 📂 Data Sources
AdventureWorks CSV datasets including:
- Calendar
- Customers
- Products
- Sales (2015–2017)
- Returns
- Territories

## 🔄 Data Flow
1. Raw CSV files ingested into **Bronze** layer
2. Data cleaned and enriched in **Silver** layer
3. Business-ready data prepared in **Gold** layer

## 🔐 Security
- Databricks connected to ADLS Gen2 using **OAuth with Service Principal**
- Secrets not exposed in code

## 📓 Notebooks
- `bronze_layer.ipynb`
- `silver_layer.ipynb`
- `gold_layer.ipynb`


## 🚀 Key Learnings
- Azure Data Lake design
- PySpark transformations
- Medallion architecture
- Real-world data engineering workflow
