# Blinkit Product Analysis using SQL

## Project Overview
This project analyzes Blinkit product data using MySQL Workbench and SQL queries to generate business insights related to product pricing, discounts, ratings, categories, and brands.

The project demonstrates:
- SQL querying skills
- Data cleaning workflow
- Business KPI analysis
- Database management
- GitHub project documentation

---

# Tools Used

- MySQL Workbench
- SQL
- Microsoft Excel
- GitHub

---

# Dataset Information

The dataset contains:
- Product names
- Categories
- Sub-categories
- Brand names
- Sale prices
- Market prices
- Product ratings

Total Records: 27,000+

---

# Data Cleaning Process

Data cleaning was performed in Microsoft Excel before importing the dataset into MySQL Workbench.

Cleaning steps included:
- Handling blank values
- Removing invalid rating values
- Verifying numeric columns
- Standardizing column names
- Checking duplicate records

---

# Database Structure

## Table Name

```sql
blinkitproducts
```

## Columns

| Column Name | Description |
|---|---|
| product_id | Unique product identifier |
| product | Product name |
| category | Product category |
| sub_category | Product sub-category |
| brand | Brand name |
| sale_price | Discounted/selling price |
| market_price | Original market price |
| type | Product type |
| rating | Product rating |

---

# SQL Concepts Used

- SELECT
- WHERE
- GROUP BY
- ORDER BY
- HAVING
- Aggregate Functions
- CASE Statements
- Business KPI Analysis

---

# Business Problems Solved

- Identified highest-rated brands
- Found products with maximum discounts
- Analyzed category-wise product distribution
- Compared pricing across categories
- Estimated brand-level revenue
- Studied premium product distribution

---

# Project Structure

```text
blinkit-product-analysis-sql/
│
├── dataset/
│   └── blinkit.csv
│
├── sql/
│   ├── create_table.sql
│   ├── data_cleaning.sql
│   └── analysis_queries.sql
│
├── screenshots/
│
├── insights.txt
│
└── README.md
```

---

# Screenshots

## 1. Dataset Preview

![Dataset Preview](screenshots/data_preview.png)

---

## 2. Table Structure

![Table Structure](screenshots/table_structure.png)

---

## 3. Total Products Analysis

![Total Products](screenshots/total_products.png)

---

## 4. Missing Values Analysis

![Missing Values Analysis](screenshots/missing_values_analysis.png)

---

## 5. Duplicate Products Check

![Duplicate Products](screenshots/duplicate_products.png)

---

## 6. Highest Rated Brands

![Highest Rated Brands](screenshots/highest_rated_brands.png)

---

## 7. Most Expensive Products

![Most Expensive Products](screenshots/most_expensive_products.png)

---

## 8. Biggest Discounts

![Biggest Discounts](screenshots/biggest_discounts.png)

---

## 9. Category-wise Product Count

![Category Product Count](screenshots/category_product_count.png)

---

## 10. Average Price by Category

![Average Price by Category](screenshots/average_price_by_category.png)

---

## 11. Best Rated Categories

![Best Rated Categories](screenshots/best_rated_categories.png)

---

## 12. Top Brands by Product Count

![Top Brands](screenshots/top_brands_by_products.png)

---

## 13. Premium Products Analysis

![Premium Products Analysis](screenshots/premium_products_analysis.png)

---

## 14. Rating Distribution

![Rating Distribution](screenshots/rating_distribution.png)

---

## 15. Average Discount Percentage

![Average Discount Percentage](screenshots/average_discount_percentage.png)

---

## 16. Top Rated Products

![Top Rated Products](screenshots/top_rated_products.png)

---

## 17. Brand Revenue Estimation

![Brand Revenue Estimation](screenshots/brand_revenue_estimation.png)

---

# Sample SQL Query

```sql
SELECT brand,
SUM(sale_price) AS estimated_revenue
FROM blinkitproducts
GROUP BY brand
ORDER BY estimated_revenue DESC;
```

---

# Key Insights

- Some brands dominate overall product listings.
- Premium products are concentrated in specific categories.
- Discount percentages vary significantly across categories.
- Highly rated brands generally maintain premium pricing.
- Revenue contribution is concentrated among top brands.

---

# Future Improvements

- Power BI Dashboard
- Python Data Analysis
- Advanced SQL Queries
- Interactive Visualizations
- Machine Learning-based Recommendations

---

# Author

Amaan Kidwai
