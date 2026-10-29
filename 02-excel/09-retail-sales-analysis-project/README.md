# Retail Sales Data Analysis Project

## Project Overview

This project analyses a sample retail sales dataset using Microsoft Excel. The goal is to transform transaction-level data into useful business insights through data validation, formulas, summary tables, charts, and a dashboard.

This project is part of my Data Analytics Learning Journey.

## Business Problem

A retail business wants to understand:
- Which products generate the highest and lowest revenue?
- Which regions generate the most revenue?
- What is the total revenue across all transactions?
- How can sales data be presented clearly to support business decisions?

## Tools Used

- Microsoft Excel
- Excel formulas and functions
- Data validation and formatting
- Charts and dashboard design

## Dataset Description

The sample dataset contains 15 transactions recorded in January 2026.

| Column | Description |
|---|---|
| Order ID | Unique transaction identifier |
| Date | Transaction date |
| Region | Region associated with the order |
| Product | Product sold |
| Category | Product category |
| Quantity | Number of units sold |
| Unit Price (₹) | Price per unit |
| Total Sales (₹) | Quantity multiplied by unit price |

**Note:** This is a practice dataset created for learning purposes, not actual company data.

## Project Workflow

1. Organised the sales dataset in Excel.
2. Checked for missing values and duplicate Order IDs.
3. Verified date, quantity, and unit-price data types.
4. Calculated transaction-level sales using `Quantity × Unit Price`.
5. Calculated total revenue using `SUM()`.
6. Analysed product and regional revenue using `SUMIF()`.
7. Created charts to compare revenue.
8. Designed a sales dashboard with key performance indicators (KPIs).
9. Interpreted results and documented business insights.

## Key Findings

- **Total revenue:** ₹2,85,750
- **Number of transactions:** 15
- **Highest-revenue product:** Laptop — ₹1,80,000
- **Lowest-revenue product:** Notebook — ₹1,750
- **Highest-revenue region:** West — ₹1,67,000
- **Lowest-revenue region:** East — ₹12,200
- **West–North revenue difference:** ₹80,000

## Excel Functions Used

- `SUM()` — calculates total revenue.
- `SUMIF()` — calculates revenue for a selected product or region.
- Relative cell references — automatically adjust formulas when copied down.

## Business Insights

1. Laptop generates the highest revenue among the six products in this dataset.
2. Notebook generates the lowest revenue among the six products.
3. West generates the highest regional revenue, while East generates the lowest.
4. Revenue depends on both quantity sold and unit price; transaction count alone does not explain revenue performance.

## Project Limitations

This analysis focuses on revenue, not profit. Product costs, operating expenses, customer details, and historical comparison data were not included. Therefore, the findings do not establish profitability, customer behaviour, or long-term sales trends.

## Learning Outcomes

Through this project, I practised:
- Validating structured data.
- Applying Excel formulas to business problems.
- Summarising data by category and region.
- Creating charts and a dashboard.
- Communicating findings and acknowledging analytical limitations.

## Future Improvements

- Add PivotTables and slicers.
- Analyse monthly and category-level trends.
- Include costs to calculate profit and profit margins.
- Expand the dataset for more advanced analysis.

---

**Project:** Data Analytics Learning Journey — Lesson 10  
**Focus:** Retail Sales Data Analysis using Excel