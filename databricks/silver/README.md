# Silver Layer – Curated Data Transformation

## Overview
The Silver Layer represents the **cleaned, standardized, and enriched data** derived from the Bronze (raw) layer.
This layer focuses on improving data quality and preparing datasets for analytical consumption.

In this project, Azure Databricks is used to process raw CSV files from Azure Data Lake Gen2 and apply transformations using PySpark.

---

## Source
- **Input**: Bronze layer data stored in ADLS Gen2  
- **Format**: CSV  
- **Ingestion Tool**: Azure Databricks (PySpark)

---

## Key Transformations
The following transformations are applied in the Silver Layer:

- Data type casting (string → integer, date, etc.)
- Removing duplicate records
- Handling null or missing values
- Standardizing column names
- Filtering invalid or corrupted records
- Adding derived columns where required

---

## Processing Logic
- Raw data is read from the Bronze container using Spark
- Transformations are applied using PySpark DataFrame APIs
- Cleaned data is written back to ADLS Gen2 in a structured format

---

## Output
- **Storage Layer**: Silver container (ADLS Gen2)
- **Format**: Parquet
- **Purpose**: Ready for analytical queries and Gold layer aggregation

---

## Technologies Used
- Azure Databricks
- PySpark
- Azure Data Lake Storage Gen2
- Azure Data Factory (upstream ingestion)

---

## Notebook
- `silver_layer.ipynb`  
  Contains end-to-end transformation logic from Bronze to Silver.

---

## Why Silver Layer?
The Silver layer ensures:
- High data quality
- Consistent schema
- Optimized storage
- Reliable foundation for business analytics

---
