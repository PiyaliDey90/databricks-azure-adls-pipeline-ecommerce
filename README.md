# 🛒 E-Commerce Data Pipeline using Azure Databricks and ADLS

## Overview
This project demonstrates an end-to-end e-commerce data pipeline built using **Azure Databricks**, **PySpark**, **ADLS Gen2**, **Delta Lake**, and **Power BI**. The solution follows the **Medallion Architecture** to transform raw data into analytics-ready datasets for reporting and business insights.

## Architecture
- **Storage Layer:** Azure Data Lake Storage Gen2 (ADLS Gen2)
- **Processing Layer:** Azure Databricks with PySpark
- **Data Format:** Delta Lake
- **Reporting Layer:** Power BI

## Project Flow
The pipeline is organized into multiple layers and processing stages:

### 1. Setup
- Catalog setup
- External volume / raw storage setup

### 2. Bronze Layer
- Ingest raw e-commerce data from source files
- Store raw data for downstream processing

### 3. Silver Layer
- Clean and standardize datasets
- Apply transformations and validations
- Prepare curated dimension and fact datasets

### 4. Gold Layer
- Build analytics-ready business tables
- Generate summary datasets and KPI-focused outputs

### 5. Dashboarding
- Build Power BI dashboard for e-commerce analytics
- Visualize revenue trends, customer behavior, and product insights

## Folder Structure
```text
databricks-azure-adls-pipeline-ecommerce/
├── 0_data/
├── 1_setup/
├── 2_medallion_processing_dim/
├── 3_medallion_processing_fact/
├── 4_dashboarding/
├── resources/
└── README.md


## Architecture Diagram
![Architecture Diagram](resources/project_architecture.png)

## Dashboard Preview
![Dashboard Preview](resources/ecommerce_analytics_report.jpg)
