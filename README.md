# End-to-End E-commerce Data Pipeline

## Overview
This project is an end-to-end data engineering pipeline built using Databricks. It processes e-commerce data from raw ingestion to analytics-ready datasets, including validation, transformation, and storage in Delta Lake.

The pipeline is designed to simulate a basic industrial data workflow.

## Tech Stack
- Databricks
- PySpark
- Delta Lake
- Databricks Volumes
- Databricks Workflows
- GitHub

## Pipeline Stages

### 1. Data Ingestion
Raw data (orders, customers, products, inventory, shipping) is loaded from Databricks Volumes.

### 2. Data Validation
Schema checks and basic business rule validations are applied to ensure data quality.

### 3. Data Enrichment
Data is transformed with additional fields such as:
- Customer segmentation
- Seasonal features
- Basic performance metrics

### 4. SCD Type 2 Implementation
Historical tracking is applied using effective and expiry dates to maintain changes over time.

### 5. Storage
Processed data is stored in Delta Lake tables across staging and final layers.

### 6. Orchestration
Databricks Workflows is used to manage sequential execution of notebooks.

## Output
- Cleaned and validated datasets
- Enriched analytical tables
- Historical tracking using SCD2
- Business-ready data for reporting

## Purpose
To practice building a structured end-to-end data pipeline using Databricks and PySpark concepts commonly used in real-world data engineering workflows.
