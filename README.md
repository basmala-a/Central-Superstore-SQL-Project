# Central Superstore SQL Analysis

## Project Overview

This project analyzes the Central Superstore retail sales dataset using MySQL. The original flat dataset was transformed into a normalized Star Schema consisting of one fact table and four dimension tables. The project then uses SQL to perform profitability analysis, customer behavior analysis, and sales trend analysis.

## Objectives

- Normalize the original flat dataset into fact and dimension tables.
- Create primary and foreign key relationships.
- Build a Star Schema for analytical reporting.
- Use SQL JOINs, subqueries, CTEs, CASE statements, and aggregate functions.
- Create reusable SQL Views for KPI analysis.
- Create a Stored Procedure for sales KPIs.
- Analyze profitability, customer behavior, and sales trends.
- Optimize analytical queries using indexes and EXPLAIN.

## Database Structure

The final analytical schema contains:

- `fact_sales`
- `dim_customer`
- `dim_product`
- `dim_location`
- `dim_ship_mode`

The original `mytable` is retained as the raw source table.

## Analysis Areas

### Profitability Analysis

- Profit and profit margin by product category
- Sub-categories below the overall profit margin
- Discount level and profitability
- Top products by profit
- Products with negative overall profit

### Customer Behavior Analysis

- Performance by customer segment
- Top customers by sales
- Customers with above-average order frequency
- Customers ordering across multiple years
- Customer value analysis

### Sales Trend Analysis

- Monthly sales and profit trends
- Sales performance over time
- Quarterly sales performance
- Sales by shipping mode over time
- Seasonal sales trends

## Additional SQL Features

The project includes:

- Primary and foreign keys
- Multiple JOIN operations
- Subqueries
- CTEs
- CASE statements
- SQL Views
- Stored Procedure
- Indexing
- Query optimization using EXPLAIN

## Project Files

- `central_superstore.sql` — Complete SQL code for the project
- `Central_Superstore_Project_Documentation.docx` — Project documentation
- `erd.png` — Database ER Diagram

## Tools

- MySQL
- MySQL Workbench
