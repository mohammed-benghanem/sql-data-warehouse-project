# Modern Data Warehouse & Analytics Platform

A comprehensive data engineering and analytics project implementing a scalable, multi-layered data warehouse from raw CSV files to business insights. This project demonstrates complete data pipeline principles, including data ingestion, transformation, dimensional modeling, and advanced analytics using the Medallion Architecture.

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project solves a common business challenge: consolidating data from disparate source systems into a unified, reliable data warehouse with actionable insights. I ingested sales data from two separate sources—a legacy ERP and a modern CRM—and transformed it through multiple layers into a clean, analysis-ready star schema.

🎯 Key Deliverables

✅ End-to-End Data Pipeline: From raw CSV ingestion to advanced analytical queries.

✅ Data Integration: Successfully merged ERP and CRM data sources with quality checks.

✅ Production-Ready Schema: Built optimized star schema for analytics.

✅ Advanced Analytics: Developed comprehensive SQL analyses for business intelligence.

✅ Data Exploration: Implemented data quality assessments and metric calculations.


📊 Analytics Capabilities

- Data Exploration: Temporal analysis, customer demographics, product catalog review.
- Business Metrics: Revenue calculations, sales performance, customer behavior analysis.
- Ranking Analysis: Top-performing products, VIP customers, product category performance.
- Magnitude Analysis: Data distribution across dimensions and key performance indicators.
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
│   └── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
├── └── analytics/                      # Advanced analytical queries and business insights
│       ├── dimensions_exploration.sql  # Data structure and temporal analysis
│       ├── measures_exploration.sql    # Key business metrics and KPI calculations
│       ├── ranking_analysis.sql        # Top performers and comparative analysis
│       ├── magnitude_analysis.sql      # Data distribution and aggregation studies
│       └── database_exploration.sql    # Data discovery and quality assessment
│
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
└── .gitignore                          # Files and directories to be ignored by Git
```
