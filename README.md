# Blinkit Product Analysis using SQL

## Project Overview
This project analyzes Blinkit product data using MySQL Workbench and SQL queries to extract meaningful business insights related to pricing, discounts, ratings, brands, and product categories.

---

## Tools Used
- MySQL Workbench
- SQL
- Microsoft Excel
- GitHub

---

## Dataset Information
The dataset contains
- Product names
- Categories
- Brands
- Sale prices
- Market prices
- Ratings

Total Records 27,000+

---

## Data Cleaning Process
Data preprocessing and cleaning were performed in Microsoft Excel before importing the dataset into MySQL Workbench.

Cleaning steps included
- Handling blank values
- Removing invalid ratings
- Checking missing values
- Standardizing column formats

---

## SQL Concepts Used
- SELECT
- WHERE
- GROUP BY
- ORDER BY
- HAVING
- Aggregate Functions
- Business KPI Analysis

---

## Business Problems Solved
- Identified highest-rated brands
- Analyzed category-wise product distribution
- Found products with maximum discounts
- Estimated brand-level revenue
- Compared pricing across categories

---

## Project Structure

```text
blinkit-product-analysis-sql
│
├── dataset
├── sql
├── screenshots
├── README.md
└── insights.txt
```

---

## Sample Query

```sql
SELECT brand,
SUM(sale_price) AS estimated_revenue
FROM blinkitproducts
GROUP BY brand
ORDER BY estimated_revenue DESC;
```

---

## Key Insights
- Some brands dominate overall product listings.
- Premium products are concentrated in specific categories.
- Discount percentages vary significantly by category.
- Higher-rated brands generally maintain premium pricing.

---

## Future Improvements
- Power BI Dashboard
- Python Data Analysis
- Advanced SQL Queries
- Interactive Visualizations

---

## Author
Amaan Kidwai
