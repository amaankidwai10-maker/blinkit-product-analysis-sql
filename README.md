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

<img width="378" height="265" alt="Image" src="https://github.com/user-attachments/assets/86f47ef4-eb15-424d-8f50-ba36e4a84b3a" />
<img width="297" height="260" alt="Image" src="https://github.com/user-attachments/assets/64da2310-0f6d-47ca-93be-ca76c6917a35" />
<img width="286" height="262" alt="Image" src="https://github.com/user-attachments/assets/90f5d5e5-97a6-474e-b4e0-fdc859401a9b" />
<img width="655" height="349" alt="Image" src="https://github.com/user-attachments/assets/77986de0-4ad2-498a-895f-d611d9cbb38c" />
<img width="253" height="254" alt="Image" src="https://github.com/user-attachments/assets/3eda139b-20c1-48d3-aa00-ef36c2d1f873" />
<img width="313" height="270" alt="Image" src="https://github.com/user-attachments/assets/602f2ae2-5db1-42e3-b4b0-f886c34b7661" />
<img width="1284" height="268" alt="Image" src="https://github.com/user-attachments/assets/ab9a5b98-8468-4f66-925d-6888f805b6cf" />
<img width="465" height="601" alt="Image" src="https://github.com/user-attachments/assets/5673b65f-b4af-4517-9fd3-7d1905ee43a7" />
<img width="351" height="240" alt="Image" src="https://github.com/user-attachments/assets/ba431116-8039-4918-8173-96101d04d9db" />
<img width="491" height="57" alt="Image" src="https://github.com/user-attachments/assets/beba9863-58c1-445a-a43e-8d94c34a4381" />
<img width="551" height="241" alt="Image" src="https://github.com/user-attachments/assets/c33f9388-675c-4aa7-ae80-1d6c7f9ba5f1" />
<img width="338" height="240" alt="Image" src="https://github.com/user-attachments/assets/e50ef6af-1351-4789-86cf-65a727cf077f" />
<img width="254" height="112" alt="Image" src="https://github.com/user-attachments/assets/e1b1400d-468a-4b62-abfc-854dc866fffd" />
<img width="427" height="250" alt="Image" src="https://github.com/user-attachments/assets/ec9809cb-795a-47af-b479-fc966d321cbd" />
<img width="266" height="245" alt="Image" src="https://github.com/user-attachments/assets/b022bc09-a15c-4eff-88cd-e082bc5d98d2" />
<img width="484" height="247" alt="Image" src="https://github.com/user-attachments/assets/d55c05b9-0980-4583-9bcb-ed1ac2a74f1a" />
<img width="611" height="74" alt="Image" src="https://github.com/user-attachments/assets/c9ddf3ae-2649-4202-be64-73e8c99f8bf9" />
