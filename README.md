# Ecommerce Data Transformation using Databricks

## Project Overview

This project demonstrates the integration of AWS S3 with Databricks to transform and store data using Delta Lake capabilities. The data is processed and stored as Delta tables, following the Medallion architecture which includes Bronze, Silver, and Gold layers. This approach ensures scalable, efficient, and reliable data processing.

## Features

- **AWS S3 Integration**: Mounting an AWS S3 bucket on Databricks for easy access to raw data.
- **Data Transformation**: Using PySpark and Spark SQL to clean and transform the data.
- **Delta Lake Storage**: Storing transformed data as Delta tables for efficient querying and data management.
- **Medallion Architecture**: Implementing a multi-layer data architecture:
  - **Bronze Layer**: Raw data ingestion.
  - **Silver Layer**: Cleaned and enriched data.
  - **Gold Layer**: Aggregated and refined data ready for analysis.

## Architecture

### Medallion Architecture

1. **Bronze Layer**:
   - Raw data is ingested from the S3 bucket and stored in its original form.
   
2. **Silver Layer**:
   - Data from the Bronze layer is cleaned, transformed, and stored in a more structured format.
   
3. **Gold Layer**:
   - Refined data from the Silver layer is further aggregated and stored for high-performance queries and analytics.

## Technologies Used

- **Databricks**: Unified analytics platform for big data processing and machine learning.
- **AWS S3**: Scalable object storage for data lakes.
- **Delta Lake**: Storage layer that brings reliability to data lakes.
- **PySpark**: Python API for Spark, enabling big data processing.
- **Spark SQL**: SQL module for querying structured data within Spark.

## Getting Started

### Prerequisites

- Databricks account 
- AWS account with access to S3

## Acknowledgements
- [Databricks](https://databricks.com/)
- [AWS S3](https://aws.amazon.com/s3/)
- [Delta Lake](https://delta.io/)


