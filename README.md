# Azure Data Engineering Project

This project demonstrates the end-to-end process of setting up data pipelines, a data lake, and a data warehouse using Microsoft Azure services. The goal is to ingest, transform, and serve sales data for a bicycle company across various product categories and subcategories.

## Project Overview

The key steps involved in this project are:

1. **Set up Azure Resources**:
   - Create an Azure Resource Group to manage all related resources.
   - Provision an Azure Storage Account with a Data Lake Storage account.
   - Create an Azure Data Factory for orchestrating data pipelines.
   - Establish an Azure Databricks workspace for data transformation.
   - Set up an Azure Synapse Analytics workspace for data warehousing and reporting.

2. **Ingest Data into the Data Lake**:
   - Implement static and dynamic data pipelines in Azure Data Factory to ingest sales data from various sources (e.g., a GitHub repository) into the Data Lake.
   - Organize the raw data into Bronze, Silver, and Gold containers within the Data Lake.

3. **Transform Data using Azure Databricks**:
   - Connect Azure Databricks to the Data Lake using a Service Principal.
   - Develop Spark notebooks to clean, transform, and enrich the sales data.
   - Write the transformed data back to the Silver and Gold containers in the Data Lake.

4. **Serve Transformed Data with Azure Synapse Analytics**:
   - Create SQL Pools (Dedicated and Serverless) in Azure Synapse to query and analyze the transformed data.
   - Establish external tables to access the data stored in the Data Lake.
   - Visualize the data using Power BI integrated with the Azure Synapse workspace.

The project utilizes the following Azure services:

- **Azure Resource Group**: Centralized management of all related resources.
- **Azure Storage Account with Data Lake Storage**: Scalable data lake to store raw, transformed, and serving-layer data.
- **Azure Data Factory**: Orchestrate data ingestion pipelines.
- **Azure Databricks**: Perform data transformation and enrichment using Spark.
- **Azure Synapse Analytics**: Provide a unified analytics platform for querying, serving, and visualizing data.
- **Power BI**: Integrate with Azure Synapse to create interactive data visualizations.

By the end of this project, you will have a robust data engineering solution that ingests, processes, and serves sales data for the bicycle company, enabling advanced analytics and reporting.

