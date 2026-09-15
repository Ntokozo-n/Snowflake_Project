
Project Overview

This project demonstrates an end-to-end relational data warehousing and analytics pipeline built in Snowflake. The primary objective is to take raw transactional and master data from non-relational CSV files, structure it within a relational star schema, enforce proper data typing, and perform core business analytics using advanced SQL queries.

The project models the core operational data of an e-commerce platform across three main entities:

  Customers (Dimension): Tracks customer profile details, locations, and signup dates across 50 records.
  Products (Dimension): Manages catalog inventory, pricing, and product categorization across 20 records.
  Orders (Fact): Captures 150 transaction logs detailing customer purchases, order dates, and quantities.

---

Key Skills Applied

**Data Engineering & Warehousing (Snowflake):** Database and schema design, stage creation, file format configuration, and direct data loading using `COPY INTO` syntax.
**Data Modeling & Type Casting:** Structuring dimension and fact tables, defining primary and foreign key relationships, and enforcing precise data types (e.g., `VARCHAR`, `INT`, `DATE`, `NUMBER(10, 2)`).
**SQL Data Cleansing & Transformation:** Handling reserved keywords (`"ORDER"`), cleaning string patterns with regular expressions (`REGEXP_REPLACE`), and transforming staging attributes into typed production schema columns.
**Relational Analytics & Aggregations:** Constructing multi-table `INNER JOIN` operations, calculating line-item revenues (`quantity * unit_price`), aggregating sales performance by customer and product category using `GROUP BY`, and leveraging `ORDER BY` and `LIMIT` clauses for top-N ranking models.






🚀 Snowflake End-to-End Data Engineering & Analytics Pipeline

 📌 Project Overview
This project demonstrates a complete end-to-end Data Engineering and Analytics pipeline built on **Snowflake**. It highlights core database administration, schema design, raw data transformation, and SQL analytical querying to solve real-world business requirements.

The pipeline ingests raw transactional data, cleans dirty formatting using regular expressions, loads structured records into strongly-typed tables, and runs multi-table JOINs and aggregations to generate actionable business reports.

---

 🛠️ Tech Stack & Key Concepts
**Data Warehouse:** Snowflake
**Language:** SQL (DDL, DML, Data Cleaning, Advanced Joins, Aggregations)
**Data Engineering Techniques:** Schema Optimization, Data Type Casting, Regular Expression Parsing (`REGEXP_REPLACE`), Data Staging & Ingestion
**Reporting & Delivery:** CSV / Excel Report Generation

---

 📁 Repository Structure
```text
├── data/
│   ├── customers.csv
│   ├── orders.csv
│   └── products.csv
├── sql/
│   ├── 01_create_tables.sql
│   ├── 02_load_and_transform_data.sql
│   └── 03_business_requirements_queries.sql
├── reports/
│   └── Query_4_Results.csv
└── README.md
