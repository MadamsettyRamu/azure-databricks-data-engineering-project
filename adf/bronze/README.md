## Bronze Layer – Raw Data Ingestion

### Overview
The Bronze layer stores raw data ingested from external sources without any transformation.

### Source
- HTTP endpoint (AdventureWorks sample data)
- Ingested using Azure Data Factory

### Pipeline
- Pipeline Name: GitToRaw
- Activity: Copy Data
- Source Dataset: ds_http
- Sink Dataset: ds_raw

### Storage
- Azure Data Lake Gen2
- Container: bronze
- Data stored in CSV format

### Purpose
- Maintain raw, immutable data
- Acts as the source of truth for downstream Silver layer transformations
