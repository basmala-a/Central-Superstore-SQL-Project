Central Superstore SQL Analysis
Project Overview
This project analyzes the Central Superstore retail sales dataset using MySQL. The original flat dataset was transformed into a normalized Star Schema consisting of one fact table and four dimension tables. The project then uses SQL to perform profitability analysis, customer behavior analysis, and sales trend analysis.

Objectives
Normalize the original flat dataset into fact and dimension tables.
Create primary and foreign key relationships.
Build a Star Schema for analytical reporting.
Use SQL JOINs, subqueries, CTEs, CASE statements, and window functions.
Create a reusable SQL View for KPI analysis.
Create a parameterized Stored Procedure.
Analyze profitability, customer behavior, and sales trends.
Optimize analytical queries using indexes and EXPLAIN.
Database Structure
The final analytical schema contains:

fact_sales
dim_customer
dim_product
dim_location
dim_ship_mode
The original mytable is retained as the raw source table.

Analysis Areas
Profitability Analysis
Profit and profit margin by product category
Sub-categories below the overall profit margin
Discount level and profitability
Top products by profit
Products with negative overall profit
Customer Behavior Analysis
Performance by customer segment
Top customers by sales
Customers with above-average order frequency
Customers ordering across multiple years
Customer value tiers
Sales Trend Analysis
Monthly sales and profit trends
Year-over-year sales growth
Quarterly sales performance
Sales by shipping mode over time
Seasonal sales trends
Additional SQL Features
The project includes:

Primary and foreign keys
Multiple JOIN operations
Subqueries
CTEs
CASE statements
Window functions
SQL View
Stored Procedure
Indexing and query optimization using EXPLAIN
Project Files
Final_Central_Superstore_Project.sql — Complete SQL code for the project
Central_Superstore_SQL_Documentation.pdf — Project documentation
ERP Diagram.png — Database/ERD diagram
Tools
MySQL
MySQL Workbench
