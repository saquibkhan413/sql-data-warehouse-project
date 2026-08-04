# SQL Data Warehouse Project

## Overview

This project demonstrates the implementation of a modern SQL-based data
warehouse using a layered architecture. Data is ingested from multiple
source systems, transformed through staging layers, and prepared for
analytics.

## Project Architecture

    Source Systems
    ├── CRM
    └── ERP
            │
            ▼
    Bronze Layer
    - Raw ingestion
    - Minimal transformations

            ▼
    Silver Layer
    - Data cleansing
    - Standardization
    - Deduplication

            ▼
    Gold Layer
    - Business-ready dimensional models
    - Reporting and analytics

## Repository Structure

    .
    ├── datasets/
    │   ├── source_crm/
    │   └── source_erp/
    ├── scripts/
    │   ├── bronze/
    │   ├── silver/
    │   └── gold/
    ├── docs/
    └── README.md

## Features

-   Multi-source data ingestion (CRM & ERP)
-   Layered ETL pipeline (Bronze, Silver, Gold)
-   SQL scripts for schema creation and data loading
-   Data cleansing and transformation
-   Analytics-ready warehouse design

## Data Sources

### CRM

-   Customer information
-   Product information
-   Sales transactions

### ERP

-   Customer master
-   Location master
-   Product category master

## Technologies

-   SQL
-   Relational Database
-   ETL
-   Data Warehousing

## Workflow

1.  Create database objects.
2.  Load raw data into Bronze layer.
3.  Transform data into Silver layer.
4.  Build Gold layer for analytics.
5.  Query business-ready tables.

## How to Run

1.  Create the database.
2.  Execute DDL scripts.
3.  Run Bronze load procedures.
4.  Execute Silver transformations.
5.  Execute Gold scripts.
6.  Validate data using analytical queries.

## Future Improvements

-   Incremental loading
-   Data quality checks
-   Automated scheduling
-   CI/CD pipeline
-   Dashboard integration (Power BI/Tableau)

## Author

**Md Saquib Khan**

------------------------------------------------------------------------

This project demonstrates end-to-end SQL data warehousing concepts,
including ETL, data modeling, and layered architecture suitable for
analytics and business intelligence.
