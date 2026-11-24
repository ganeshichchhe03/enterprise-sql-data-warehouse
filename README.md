# Data Warehouse and Analytics Project

## Overview
This project demonstrates the implementation of a modern Data Warehouse solution using SQL Server. The project follows the Medallion Architecture approach (Bronze, Silver, and Gold layers) to transform raw ERP and CRM data into analytics-ready datasets for business reporting and decision-making.

## Objectives
- Build a scalable Data Warehouse using SQL Server.
- Develop ETL pipelines for data ingestion and transformation.
- Improve data quality through cleansing and standardization.
- Design analytical data models using Star Schema.
- Generate insights related to customer behavior, product performance, and sales trends.

## Architecture

### Bronze Layer
- Loaded raw ERP and CRM datasets from CSV files into SQL Server.
- Preserved source data without modifications for traceability.

### Silver Layer
- Performed data cleaning and transformation.
- Removed duplicates and handled missing values.
- Standardized formats and integrated multiple source systems.

### Gold Layer
- Created business-ready datasets.
- Designed Fact and Dimension tables.
- Implemented Star Schema for analytical reporting.

## ETL Process
1. Extract data from ERP and CRM CSV files.
2. Load raw data into Bronze Layer.
3. Clean and transform data in Silver Layer.
4. Build analytical models in Gold Layer.
5. Run SQL-based analytics for reporting and insights.

## Technologies Used
- SQL Server
- SQL Server Management Studio (SSMS)
- T-SQL
- Data Warehousing
- ETL Development
- Star Schema Modeling
- Git & GitHub

## Database Design
The warehouse consists of:
- Fact Sales
- Dim Customer
- Dim Product
- Dim Date

These tables support efficient analytical queries and reporting.

## Key Skills Demonstrated
- Data Warehousing
- SQL Development
- ETL Pipeline Development
- Data Modeling
- Data Cleansing
- Star Schema Design
- Data Analytics

## Business Analysis
Using SQL queries, the project provides insights into:
- Customer purchasing behavior
- Product performance analysis
- Sales trends
- Revenue reporting
- Business KPIs

## Repository Structure

```text
datasets/      -> Source CSV files
docs/          -> Architecture and design documents
scripts/       -> ETL and transformation scripts
tests/         -> Data quality validation scripts
```

## Results
Successfully developed an end-to-end Data Warehouse solution that converts raw business data into structured, analytics-ready information for reporting and decision-making.

## Author
Ganesh Ichchhe
