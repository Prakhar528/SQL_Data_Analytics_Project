# SQL Data Analytics Project

## Project Overview

This project demonstrates end-to-end SQL data analysis using Microsoft SQL Server. It focuses on transforming raw sales data into meaningful business insights through exploratory analysis, window functions, aggregations, segmentation techniques, and reusable reporting views.

The project follows a structured analytics workflow, progressing from trend analysis to business reporting while applying SQL best practices.

---

## Objectives

- Analyze sales performance over time
- Identify business growth trends
- Perform cumulative and comparative analysis
- Segment customers based on purchasing behavior
- Generate reusable customer and product reports
- Practice advanced SQL concepts used in real-world analytics

---

## Tech Stack

- **Database:** Microsoft SQL Server
- **Language:** SQL (T-SQL)
- **IDE:** SQL Server Management Studio (SSMS)

---

## Project Structure

```
SQL_Data_Analytics_Project/
│
├── scripts/
│   ├── changes_over_time.sql
│   ├── cumulative_analysis.sql
│   ├── performance_analysis.sql
│   ├── part_to_whole_analysis.sql
│   ├── data_segmentation.sql
│   ├── customer_report.sql
│   └── product_report.sql
│
├── datasets/      
│   ├── gold.dim_customers.csv
│   ├── gold.dim_products.csv
│   └── gold.fact_sales.csv
│
├── .gitignore
└── README.md
```

---

# Analyses Performed

## 1. Changes Over Time Analysis

Analyzes yearly business performance by calculating:

- Total Sales
- Total Customers
- Total Quantity Sold

**Concepts Used**

- GROUP BY
- DATE Functions
- Aggregation Functions

---

## 2. Cumulative Analysis

Calculates cumulative business metrics to understand long-term growth.

Includes:

- Running Total Sales
- Moving Average Price

**Concepts Used**

- Window Functions
- SUM() OVER()
- AVG() OVER()

---

## 3. Performance Analysis

Evaluates business performance across different dimensions to identify top-performing areas.

**Concepts Used**

- Aggregations
- Ranking
- CASE Statements

---

## 4. Part-to-Whole Analysis

Determines each category's contribution to overall business performance.

**Concepts Used**

- Percentage Calculations
- Window Functions
- Aggregations

---

## 5. Data Segmentation

Groups customers into meaningful segments based on purchasing behavior.

Examples include:

- High-value customers
- Regular customers
- New customers

**Concepts Used**

- CASE Statements
- Aggregations
- Business Rules

---

# Reports

## Customer Report

A reusable SQL View that summarizes customer performance.

Metrics include:

- Customer Information
- Age Group
- Customer Segment
- Total Orders
- Total Sales
- Total Quantity
- Total Products Purchased
- Recency
- Customer Lifespan
- Average Order Value
- Average Monthly Spend

---

## Product Report

A reusable SQL View that summarizes product performance.

Metrics include:

- Product Sales
- Total Orders
- Quantity Sold
- Revenue
- Product Performance Indicators
- Product Segmentation

---

# SQL Concepts Demonstrated

- Common Table Expressions (CTEs)
- Window Functions
- Aggregate Functions
- CASE Expressions
- Views
- Joins
- Date Functions
- Ranking Functions
- Business Segmentation
- Running Totals
- Moving Averages

---

## How to Run

1. Clone the repository.

2. Open **SQL Server Management Studio (SSMS)**.

3. Run the SQL scripts in the `scripts` folder .

> **Note:** Before running `00_init_database.sql`, update the dataset directory path to match the location of the dataset on your system.

4. Query the generated report views:

```sql
SELECT *
FROM gold.report_customers;

SELECT *
FROM gold.report_products;
```

---

# Learning Outcomes

Through this project, I practiced:

- Writing clean and modular SQL
- Building reusable reporting views
- Performing business-focused data analysis
- Applying advanced SQL window functions
- Designing maintainable SQL scripts
- Translating raw data into actionable insights

---

# Author

**Prakhar Naudiyal**
