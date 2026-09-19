# Central Superstore SQL Project

## 📌 Project Overview

Central Superstore is a MySQL database project based on a Superstore-style sales dataset.

The project transforms raw sales data into a structured analytical database using normalization and a Star Schema design.

The database was implemented using MySQL and includes data validation, dimensional modeling, advanced SQL analysis, views, a stored procedure, and performance optimization.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Clean and validate the raw sales data.
- Normalize the dataset into fact and dimension tables.
- Create primary key and foreign key relationships.
- Build a Star Schema model.
- Perform advanced SQL analysis.
- Use JOINs, subqueries, CTEs, CASE statements, and aggregate functions.
- Create reusable SQL Views.
- Create a Stored Procedure for sales KPIs.
- Improve query performance using indexes.
- Analyze sales, profit, customers, products, categories, locations, and shipping performance.

---

## 🗂️ Project Structure

```text
Central-Superstore-SQL-Project/
│
├── README.md
│
├── SQL/
│   └── central_superstore.sql
│
├── Documentation/
│   └── Central_Superstore_Project_Documentation.docx
│
└── ERD/
    └── erd.png
📊 Fact Table
fact_sales

The fact table contains transactional sales information and foreign keys connecting the fact table to the dimension tables.

Main columns:

sales_key
row_id
order_id
customer_key
product_key
location_key
ship_mode_key
order_date
ship_date
sales
quantity
discount
profit
📦 Dimension Tables
dim_customer

Contains customer information:

customer_key
customer_id
customer_name
segment
dim_product

Contains product information:

product_key
product_id
product_name
category
sub_category
dim_location

Contains geographical information:

location_key
country
city
state
postal_code
region
dim_ship_mode

Contains shipping mode information:

ship_mode_key
ship_mode
🔑 Database Relationships

The fact_sales table is connected to the dimension tables using foreign keys:

customer_key
product_key
location_key
ship_mode_key
🧹 Data Validation

The project includes data validation checks such as:

Total number of records.
NULL value checks.
Distinct customer count.
Distinct product count.
Distinct order count.
Distinct shipping modes.
Distinct categories.
Distinct sub-categories.
Distinct regions.
Duplicate Row_ID checks.
🔄 Data Loading Process

The project follows this process:

Raw Data
   ↓
mytable
   ↓
Data Validation
   ↓
Dimension Tables
   ↓
fact_sales
   ↓
SQL Analysis
   ↓
Views & Stored Procedure
   ↓
Optimization
🔍 Advanced SQL Analysis

The project uses advanced SQL techniques including:

JOIN
GROUP BY
HAVING
CASE
Subqueries
CTEs
Aggregate Functions
Date Functions
ORDER BY
LIMIT
ROUND
NULLIF
Analysis Areas
Total Sales
Total Profit
Total Quantity
Total Orders
Total Customers
Profit Margin
Sales and Profit by Category
Sales by Segment
Top Customers
Sales and Profit by State
Monthly Sales Trend
Loss-Making Products
Shipping Duration
Discount Analysis
👁️ SQL Views
vw_category_kpis

Provides category-level KPIs including:

Total Sales
Total Quantity
Total Profit
Profit Margin
vw_customer_behavior

Provides customer-level behavior metrics including:

Customer information
Number of orders
Quantity
Sales
Profit
Profit Margin
⚙️ Stored Procedure
sp_sales_kpis

The stored procedure provides the main overall sales KPIs:

Total Orders
Total Customers
Total Units
Total Sales
Total Profit
Profit Margin

Execute it using:

CALL sp_sales_kpis();
🚀 Performance Optimization

Indexes were created on commonly used columns:

customer_key
product_key
location_key
order_date
ship_date
ship_mode_key
order_id

The project also uses EXPLAIN to inspect query execution plans.

🗺️ ER Diagram

The database structure and relationships are represented in the ER Diagram available in the ERD folder.

▶️ How to Run
Install MySQL and MySQL Workbench.
Open the SQL script from the SQL folder.
Execute the script from the beginning.
The database central_superstore will be created.
The raw data will be loaded into mytable.
The dimension tables will be created and populated.
The fact_sales table will be created and populated.
The analytical queries, views, stored procedure, and indexes will be created.
📚 Documentation

Detailed project documentation is available in the Documentation folder.

🛠️ Technologies Used
MySQL
MySQL Workbench
SQL
GitHub
📌 Project Summary

This project demonstrates how raw sales data can be transformed into a structured analytical database using normalization, Star Schema design, advanced SQL analysis, reusable database objects, and performance optimization.
