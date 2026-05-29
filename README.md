# 🛒 Northwind Sales Analysis — SQL Project

A end-to-end business intelligence analysis of the Northwind database using SQL.  
This project simulates a real-world analyst task: exploring sales data to uncover revenue drivers, performance gaps, and customer behavior insights.

---

## 📌 Project Overview

**Database:** Northwind (MySQL)  
**Tool:** MySQL Workbench  
**Skills Demonstrated:** JOINs, Aggregations, Subqueries, Window Functions, CASE statements, Date Functions

---

## 🎯 Business Questions Answered

| # | Question | Key Concept |
|---|----------|-------------|
| 1 | Which products generate the most revenue? | JOIN, SUM, GROUP BY |
| 2 | How did sales trend month over month? | DATE functions, GROUP BY |
| 3 | Which countries drive the most orders and revenue? | Multi-table JOIN, ORDER BY |
| 4 | Which employees are above/below average in sales? | Subquery, Window Function, CASE |
| 5 | How many customers are one-time vs repeat buyers? | Nested Subquery, CASE, Window Function |

---

## 📊 Key Findings

### 1. 🏆 Top Products by Revenue
- **Côte de Blaye** dominates with **$149,984** in revenue — nearly double the second-ranked product.
- The top 5 products are all food & beverage items, suggesting a strong core category.
- **Business Insight:** High dependency on a single SKU is a potential risk — if Côte de Blaye underperforms, overall revenue takes a significant hit.

### 2. 📈 Monthly Sales Trend
- **1997 was the peak year**, with a **191% growth** over 1996.
- **April 1998** recorded the highest single month at **$134,631**.
- Note: 1996 data starts from August and 1998 data ends mid-year — raw year-over-year comparisons should account for these incomplete periods.

### 3. 🌍 Sales by Country
- **USA leads** with 352 orders and $263,567 in revenue.
- **Austria** ranks 6th in orders but **3rd in revenue** — indicating a high average order value and a premium customer segment worth prioritizing.
- **Brazil** has high order volume but relatively low revenue per order, suggesting lower-value transactions.

### 4. 👨‍💼 Employee Sales Performance
- **Margaret Peacock** is the top performer at **$250,187** — 66% above the company average of $150,495.
- **Steven Buchanan** recorded the lowest sales at **$75,568** — less than half the company average.
- 5 out of 9 employees fall below average, suggesting an opportunity for targeted sales coaching or performance review.

### 5. 🔄 Customer Retention
- **98%+ of customers are repeat buyers** — only 1 one-time buyer was identified out of the entire customer base.
- This indicates exceptionally strong customer loyalty and retention.
- **Business Insight:** Retention strategy is working well; growth efforts should focus on acquiring new customers rather than re-engaging existing ones.

---

## 📁 Project Structure

```
northwind-sales-analysis/
│
├── README.md
│
├── queries/
│   ├── 01_top_products_by_revenue.sql
│   ├── 02_monthly_sales_trend.sql
│   ├── 03_sales_by_country.sql
│   ├── 04_employee_performance.sql
│   └── 05_customer_retention.sql
│
└── outputs/
    └── screenshots/
        ├── 01_top_products.png
        ├── 02_monthly_trend.png
        ├── 03_sales_by_country.png
        ├── 04_employee_performance.png
        └── 05_customer_retention.png
```

---

## 💡 SQL Concepts Used

- **JOINs** — combining data across multiple tables
- **Aggregate Functions** — SUM, COUNT, AVG, ROUND
- **GROUP BY / HAVING** — segmenting and filtering grouped data
- **Subqueries** — using query results as input to outer queries
- **Window Functions** — `AVG() OVER()` for cross-row calculations without collapsing results
- **CASE Statements** — applying conditional business logic inside queries
- **Date Functions** — `YEAR()`, `MONTH()`, `MONTHNAME()` for time-based analysis

---

## 🚀 How to Run

1. Import the Northwind database into MySQL Workbench
2. Open any `.sql` file from the `queries/` folder
3. Run the query and view results in the Result Grid

---

## 👤 Author

**[Haytham Alghamdi]**  
Fresh Graduate — Data Analyst  
📧 haythamabdullahgh@gmail.com  
🔗 [LinkedIn Profile]([https://linkedin.com/in/yourprofile](https://www.linkedin.com/in/haytham-alghamdi-68b890263/))
