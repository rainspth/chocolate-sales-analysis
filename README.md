# Chocolate Sales Analysis

## Project Overview
This project analyzes global chocolate sales data to understand purchasing behavior and revenue distribution across countries. The objective is to identify sales patterns, vendor performance, and market concentration risks using data analytics and visualization.

## Tools
- SQL
- Power BI
- Statistical Analysis

## Data Workflow
1. Cleaned and transformed raw sales data using SQL
2. Aggregated revenue metrics by country and vendor
3. Built an interactive Power BI dashboard
4. Analyzed vendor concentration and regional performance

## Key Insights
- Analysis of India’s sales data revealed that a single-country vendor generated **3.6× higher revenue** than the global top-ranked player, highlighting hyper-local market concentration.
- Top-performing vendors showed more balanced revenue distribution across regions.
- Certain countries demonstrated higher chocolate purchasing power.

## Dashboard Preview
![Chocolate Sales Dashboard](images/Chocolate dashboard.png)
## Sample SQL Queries

### Total sales by Country
```sql
SELECT country, SUM(amount) AS total_sales
FROM chocolate_sales
GROUP BY country
ORDER BY total_sales DESC;
