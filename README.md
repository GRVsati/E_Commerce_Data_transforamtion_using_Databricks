# Ecommerce Data Transformation using Databricks

## Overview
This project focuses on transforming ecommerce data using Databricks, leveraging AWS S3 for storage and Delta Lake for efficient data processing. The data transformation follows the Medallion Architecture, moving data through different layers (bronze, silver, gold) for various levels of processing and analysis.

## Architecture
The architecture of this project follows the Medallion Architecture:

1. **Bronze Layer**: Raw data is ingested and stored as Delta tables in the bronze layer.
2. **Silver Layer**: Data is transformed and cleaned as per requirements and stored in Delta tables in the silver layer.
3. **Gold Layer**: Further processing may occur, and the data is stored in Delta tables in the gold layer for analysis.

## Technologies Used
- Databricks
- AWS S3
- Delta Lake

## Setup Instructions
1. **Create S3 Bucket**: Set up an S3 bucket on AWS to store the data.
2. **IAM User Configuration**: Create an IAM user with appropriate permissions to access the S3 bucket.
3. **Mount S3 Bucket in Databricks**: Use the IAM user credentials to mount the S3 bucket in Databricks.When we mount an S3 bucket in Databricks, it create a logical link between the S3 bucket and a mount point within our Databricks file system. This allows us to access the files in the S3 bucket using standard 
file system commands directly from Databricks.
4. **Data Loading**: Load the raw data into Databricks and save it as Delta tables in the bronze layer.
5. **Data Transformation**: Transform the data using Pyspark and SparkSql as required and save it as Delta tables in the silver layer.After that combine all the tables to form OBT(One Big table).
6. **Further Processing (Optional)**: Perform additional processing and save the data in the gold layer as OBT

## Usage
1. **Data Analysis**: Access the data stored in the gold layer for further analysis using various services or tools like PowerBI or Tableau.

## Contributing
Contributions to improve this project are welcome. Please fork the repository and submit pull requests with your proposed changes.


## Acknowledgements
- [Databricks](https://databricks.com/)
- [AWS S3](https://aws.amazon.com/s3/)
- [Delta Lake](https://delta.io/)


