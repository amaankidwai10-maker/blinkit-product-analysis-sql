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

<div align="center">

# Database Setup & Data Import

## 1. Dataset Preview

<img width="655" height="349" alt="Dataset Preview" src="https://github.com/user-attachments/assets/77986de0-4ad2-498a-895f-d611d9cbb38c" />

---

## 2. Table Structure

<img width="611" height="74" alt="Table Structure" src="https://github.com/user-attachments/assets/c9ddf3ae-2649-4202-be64-73e8c99f8bf9" />

---

## 3. Total Products Analysis

<img width="491" height="57" alt="Total Products" src="https://github.com/user-attachments/assets/beba9863-58c1-445a-a43e-8d94c34a4381" />

---

# Data Cleaning Analysis

## 4. Missing Values Analysis

<img width="551" height="241" alt="Missing Values Analysis" src="https://github.com/user-attachments/assets/c33f9388-675c-4aa7-ae80-1d6c7f9ba5f1" />

---

## 5. Duplicate Products Check

<img width="465" height="601" alt="Duplicate Products Check" src="https://github.com/user-attachments/assets/5673b65f-b4af-4517-9fd3-7d1905ee43a7" />

---

# Business KPI Analysis

## 6. Highest Rated Brands

<img width="378" height="265" alt="Highest Rated Brands" src="https://github.com/user-attachments/assets/86f47ef4-eb15-424d-8f50-ba36e4a84b3a" />

---

## 7. Most Expensive Products

<img width="297" height="260" alt="Most Expensive Products" src="https://github.com/user-attachments/assets/64da2310-0f6d-47ca-93be-ca76c6917a35" />

---

## 8. Biggest Discounts

<img width="286" height="262" alt="Biggest Discounts" src="https://github.com/user-attachments/assets/90f5d5e5-97a6-474e-b4e0-fdc859401a9b" />

---

## 9. Category-wise Product Count

<img width="313" height="270" alt="Category Product Count" src="https://github.com/user-attachments/assets/602f2ae2-5db1-42e3-b4b0-f886c34b7661" />

---

## 10. Average Price by Category

<img width="351" height="240" alt="Average Price by Category" src="https://github.com/user-attachments/assets/ba431116-8039-4918-8173-96101d04d9db" />

---

## 11. Best Rated Categories

<img width="338" height="240" alt="Best Rated Categories" src="https://github.com/user-attachments/assets/e50ef6af-1351-4789-86cf-65a727cf077f" />

---

## 12. Top Brands by Product Count

<img width="427" height="250" alt="Top Brands by Product Count" src="https://github.com/user-attachments/assets/ec9809cb-795a-47af-b479-fc966d321cbd" />

---

## 13. Premium Products Analysis

<img width="266" height="245" alt="Premium Products Analysis" src="https://github.com/user-attachments/assets/b022bc09-a15c-4eff-88cd-e082bc5d98d2" />

---

## 14. Rating Distribution

<img width="254" height="112" alt="Rating Distribution" src="https://github.com/user-attachments/assets/e1b1400d-468a-4b62-abfc-854dc866fffd" />

---

## 15. Average Discount Percentage

<img width="484" height="247" alt="Average Discount Percentage" src="https://github.com/user-attachments/assets/d55c05b9-0980-4583-9bcb-ed1ac2a74f1a" />

---

## 16. Top Rated Products

<img width="253" height="254" alt="Top Rated Products" src="https://github.com/user-attachments/assets/3eda139b-20c1-48d3-aa00-ef36c2d1f873" />

---

## 17. Brand Revenue Estimation

<img width="1284" height="268" alt="Brand Revenue Estimation" src="https://github.com/user-attachments/assets/ab9a5b98-8468-4f66-925d-6888f805b6cf" />

</div>
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
