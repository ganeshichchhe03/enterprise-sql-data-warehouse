# 🚀 Data Warehouse & Analytics Project

## 📋 Overview

This project demonstrates the implementation of a modern Data Warehouse using SQL Server. The solution follows the Medallion Architecture (Bronze, Silver, and Gold layers) to transform raw CRM and ERP data into clean, business-ready datasets for reporting and analytics.

The project covers the complete data warehousing lifecycle, including data ingestion, transformation, cleansing, data quality validation, and analytical modeling.

---

## 🎯 Project Objectives

- Build a scalable SQL Server Data Warehouse.
- Integrate CRM and ERP data sources.
- Develop automated ETL pipelines using Stored Procedures.
- Apply data cleansing and transformation rules.
- Create analytics-ready datasets.
- Enable business reporting and decision-making.

---

## 🏗️ Data Architecture

The project follows the Medallion Architecture pattern:

### Bronze Layer (Raw Data)
- Loads source data from CSV files.
- Stores data without business transformations.
- Preserves original source records.
- Acts as the landing zone for CRM and ERP datasets.

### Silver Layer (Cleansed Data)
- Standardizes data formats.
- Removes duplicates.
- Handles missing or invalid values.
- Applies business rules.
- Performs data quality validation.
- Creates clean and consistent datasets.

### Gold Layer (Business Layer)
- Business-ready analytical datasets.
- Fact and Dimension tables.
- Star Schema design.
- Optimized for reporting and analytics.

---

## 📊 Data Sources

### CRM Data
- Customer Information
- Product Information
- Sales Transactions

### ERP Data
- Customer Demographics
- Customer Location Data
- Product Category Information

---

## ⚙️ ETL Pipeline

The ETL process is implemented using SQL Server Stored Procedures.

### Bronze Layer Processing

The Bronze loading procedure:

- Truncates existing tables.
- Loads CSV files using BULK INSERT.
- Imports CRM and ERP source data.
- Tracks execution duration.
- Logs processing information.
- Handles loading errors using TRY-CATCH.

### Silver Layer Processing

The Silver loading procedure performs:

#### Customer Data Transformation
- Customer deduplication using ROW_NUMBER().
- Gender normalization.
- Marital status standardization.
- Data cleansing and trimming.

#### Product Data Transformation
- Product category extraction.
- Product code standardization.
- Product line mapping.
- Historical product date handling.

#### Sales Data Validation
- Invalid date correction.
- Sales amount validation.
- Price recalculation.
- Missing value handling.

#### ERP Data Standardization
- Customer ID normalization.
- Country name standardization.
- Gender normalization.
- Future date validation.

---

## 🧹 Data Quality Checks

The ETL pipeline implements multiple quality controls:

- Duplicate record removal.
- Null value handling.
- Invalid date correction.
- Standardized code mapping.
- Sales value validation.
- Customer data cleansing.
- Country code normalization.
- Product category standardization.

---

## 🗄️ Database Schemas

### Bronze Schema

#### CRM Tables
- crm_cust_info
- crm_prd_info
- crm_sales_details

#### ERP Tables
- erp_loc_a101
- erp_cust_az12
- erp_px_cat_g1v2

### Silver Schema

#### CRM Tables
- crm_cust_info
- crm_prd_info
- crm_sales_details

#### ERP Tables
- erp_loc_a101
- erp_cust_az12
- erp_px_cat_g1v2

---

## 🛠️ Technologies Used

- SQL Server
- SQL Server Management Studio (SSMS)
- T-SQL
- Data Warehousing
- ETL Development
- Stored Procedures
- BULK INSERT
- Data Modeling
- Git
- GitHub

---

## 📁 Project Structure

```text
data-warehouse-project/
│
├── datasets/
│   ├── source_crm/
│   └── source_erp/
│
├── scripts/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── docs/
│
├── README.md
│
└── LICENSE
```

---

## 💡 Key Skills Demonstrated

- Data Warehousing
- SQL Development
- ETL Pipeline Design
- Data Cleansing
- Data Quality Management
- Data Integration
- Stored Procedure Development
- SQL Performance Optimization
- Data Modeling
- Business Intelligence Foundations

---

## 📈 Business Value

This project transforms raw operational data into a structured analytical platform capable of supporting:

- Customer Analytics
- Product Analytics
- Sales Reporting
- Performance Measurement
- Business Decision Making

---

## 👨‍💻 Author

**Ganesh Ichchhe**
- GitHub: https://github.com/ganeshichchhe03

---

## ⭐ Future Enhancements
- Power BI Dashboards
