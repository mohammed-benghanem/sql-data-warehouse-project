# Modern Data Warehouse Implementation

A hands-on data engineering project building a scalable, multi-layered data warehouse from raw CSV files. This implementation demonstrates core data pipeline principles, including data ingestion, transformation, and dimensional modeling using the Medallion Architecture.

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project solves a common business challenge: consolidating data from disparate source systems into a unified, reliable data warehouse. I ingested sales data from two separate sources—a legacy ERP and a modern CRM—and transformed it through multiple layers into a clean, analysis-ready star schema.

✅ Full Data Pipeline: From raw CSV ingestion to structured dimensional models.
✅ Data Integration: Successfully merged ERP and CRM data sources.
✅ Quality Assurance: Implemented data cleansing and standardization.
✅ Production-Ready Schema: Built a optimized star schema for analytics.

---
## 📂 Repository Structure
```
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── data_architecture.drawio        # Draw.io file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.drawio                # Draw.io file for the data flow diagram
│   ├── data_models.drawio              # Draw.io file for data models (star schema)
│   ├── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
└── .gitignore                          # Files and directories to be ignored by Git
```
