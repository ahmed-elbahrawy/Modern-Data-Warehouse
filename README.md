:

Modern Data Warehouse for Bicycle Sales Analytics
This project delivers an end-to-end Data Warehouse (DWH) solution for a fictional bicycle sales operation using the Microsoft BI stack. It enables advanced analytics and executive-level reporting across sales, inventory, and operational efficiency using the Medallion Architecture (ODS → STG → DWH).

🚴♂️ Project Overview
Purpose: Enable robust analytical insights and BI reporting for sales and inventory operations.

Architecture: Medallion Architecture (ODS → STG → DWH).

Tools Used:

Azure SQL Server

SQL Server Management Studio (SSMS)

SQL Server Integration Services (SSIS)

SQL Server Analysis Services (SSAS)

Power BI

Visual Studio 2019

📊 Data Model
Conceptual Schema: Star Schema

Fact Tables:

fact_order_items

fact_stocks

Dimension Tables:

dim_products

dim_categories

dim_brands

dim_customers

dim_stores

dim_staff

dim_date

ERD:
Included in the repo: conceptual-model.jpg

⚙️ ETL Pipeline (SSIS)
Modular ETL packages for ODS → STG and STG → DWH.

Incremental loading for orders and customer data.

Data cleansing, standardization, validation, and referential integrity.

Logging and configuration for scalable execution.

🗄️ DWH Backup
Cleaned, validated production-ready schema.

.bak backup included (DWH_Bicycle.bak).

📈 Analytics Model (SSAS)
Clean tabular model built on processed DWH tables.

Measures & Calculated Columns include:

Total Sales Amount

Total Discount

Net Sales

Number of Orders

Repeat Customer Rate

Late Shipments Count

Out of Stock Items

📊 Power BI Dashboard
Interactive dashboard with real-time analytics, connected to SSAS model.

Pages:

Landing Page: Navigation & project overview.

Main Analytics: Sales breakdown by category, brand, store, employee KPIs, revenue trends.

📂 Project Structure
text
/
├── DWH_Bicycle.bak           # DWH backup file
├── conceptual-model.jpg      # ERD and data model
├── SSIS/                     # ETL packages
├── SSAS/                     # Data model definitions
├── PowerBI/                  # Dashboard files
└── README.md                 # Project description
🚀 Getting Started
Restore the DWH using the provided .bak file.

Deploy SSIS Packages using SQL Server Data Tools or Visual Studio.

Process the SSAS Model for analytics.

Open Power BI Report and connect to the SSAS data source.

🥇 Skills & Features
Modern, modular ETL/ELT development.

Star schema modeling for KPI analytics.

Incremental processing & error handling.

Integration with Azure SQL & end-to-end Microsoft BI stack.

Real-time, interactive dashboards powered by Power BI.

Made with passion by Ahmed Elbahrawy

