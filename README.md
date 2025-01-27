# Walmart BI Project

## Project Overview
This project focuses on analyzing Walmart's sales data to derive valuable insights that drive strategic decisions. By leveraging modern Business Intelligence (BI) tools, the project explores key sales trends, customer behaviors, and product performance across Walmart's various stores and product categories.

## Table of Contents
- [Project Objectives](#project-objectives)
- [Data Sources](#data-sources)
- [ETL Process](#etl-process)
- [Data Warehousing](#data-warehousing)
- [Data Modeling](#data-modeling)
- [Data Visualization](#data-visualization)
- [Tools and Technologies](#tools-and-technologies)
- [Authors](#authors)
- [Contact Information](#contact-information)

## Project Objectives
1. Identify the store locations generating the highest profit.
2. Analyze sales performance across different time periods.
3. Determine the most profitable product categories and customer segments.
4. Explore variations in shipping costs across different locations.
5. Provide actionable recommendations for improving sales and reducing costs.

## Data Sources
The project utilizes diverse datasets from various formats:
- **CSV Files**: Grocery, Product, and Store Status datasets.
- **Excel Files**: Client demographics, sales transactions, and historical retail data.
- **JSON Files**: GeoJSON data for Walmart store locations.
- **APIs**:
  - HuggingFace: Store information (opening dates, locations, etc.).
  - Kaggle: Weekly sales data with economic indicators.

## ETL Process
1. **Data Extraction**:
   - Data gathered from CSV, Excel, JSON files, and APIs.
   - Logical and physical extraction methods used.
2. **Data Transformation**:
   - Datasets merged using common columns (e.g., SKU).
   - Cleaning steps include handling duplicates, filling missing values, standardizing column names, and data type conversions.
3. **Data Loading**:
   - Transformed data stored in Azure Blob Storage and Snowflake staging tables.

## Data Warehousing
- **Platform**: Snowflake
- **Schema Design**:
  - **Fact Table**: `Sales_Fact` (transactional data).
  - **Dimension Tables**: Product, Customer, Shipping, Time, and Promotion dimensions.
- **Queries**: ROLAP for real-time analysis.

## Data Modeling
A star schema was designed to optimize query performance. Key attributes:
- **Fact Table**: Measures like sales, profit, shipping costs, etc.
- **Dimension Tables**: Attributes for product details, customer demographics, shipping info, and promotional offers.

## Data Visualization
- **Tools**: Power BI (Desktop version)
- Key insights visualized through charts:
  - Donut charts for store performance.
  - Line graphs for sales trends.
  - Bar charts for product and category profitability.
  - Demographics and shipping cost distributions.

## Tools and Technologies
- **Programming and Data Tools**: Python, Google Colab, Azure Blob Storage, Snowflake, Power BI.
- **APIs**: HuggingFace, Kaggle.
- **Data Formats**: CSV, Excel, JSON.

## Authors
- **Saif Chouaya**
- **Eya Hafsi**
- **Mohamed Rayen Fadhlaoui**
- **Sayda Ouaddar**

## Contact Information
For any inquiries, feel free to contact us:
- Saif Chouaya: [saif.chouaya@tbs.u-tunis.tn](mailto:saif.chouaya@tbs.u-tunis.tn)
- Eya Hafsi: [e.hafsii@gmail.com](mailto:e.hafsii@gmail.com)
- Mohamed Rayen Fadhlaoui: [fadhlaouirayen@gmail.com](mailto:fadhlaouirayen@gmail.com)
- Sayda Ouaddar: [Saydaouaddar@gmail.com](mailto:Saydaouaddar@gmail.com)