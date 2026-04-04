# 🍕 Pizza Sales Analysis using SQL

> A complete MySQL-based data analysis project covering 13 SQL queries across Basic, Intermediate, and Advanced levels on a real-world pizza restaurant dataset.

---

## 📌 Project Overview

This project analyzes a pizza restaurant's sales data using **MySQL**. The goal is to extract meaningful business insights — like revenue, top-selling pizzas, peak hours, and category-wise performance — using structured SQL queries.

**GitHub Profile:** [github.com/8859384101](https://github.com/8859384101)

---

## 🗃️ Database Schema

The database consists of **4 tables:**

```
orders            order_details         pizzas            pizza_types
-----------       ---------------       ----------        ---------------
order_id (PK)     order_details_id (PK) pizza_id (PK)     pizza_type_id (PK)
date              order_id (FK)         pizza_type_id (FK) name
time              pizza_id (FK)         size              category
                  quantity              price             ingredients
```

### Relationships
- `orders` → `order_details` : One order can have many items (1:N)
- `pizza_types` → `pizzas` : One type can have many size variants (1:N)
- `order_details` ↔ `pizzas` : Joined via `pizza_id`

---

## 📊 Key Insights

| Metric | Value |
|--------|-------|
| 💰 Total Revenue | $817,860.05 |
| 📦 Total Orders | 21,350 |
| 🍕 Most Ordered Pizza | The Classic Deluxe Pizza (2,453 orders) |
| 👑 Highest Priced Pizza | The Greek Pizza ($35.95) |
| 📏 Most Popular Size | Large (L) — 18,526 orders |
| 🏆 Top Revenue Pizza | The Thai Chicken Pizza ($43,434.25) |
| ⏰ Peak Order Hour | 12 PM (2,520 orders) |
| 📈 Avg Pizzas/Day | ~138 pizzas |

---

## 📁 Project Structure

```
pizza-sales-sql/
│
├── queries/
│   ├── basic_queries.sql           # Q1 to Q5
│   ├── intermediate_queries.sql    # Q6 to Q10
│   └── advanced_queries.sql        # Q11 to Q13
│
├── Pizza_Sales_SQL_Analysis.pptx   # Full presentation with queries & outputs
└── README.md
```

---

## 🔍 SQL Queries — Summary

### 🟢 Basic (Q1–Q5)

| # | Question |
|---|----------|
| Q1 | Retrieve the total number of orders placed |
| Q2 | Calculate the total revenue generated from pizza sales |
| Q3 | Identify the highest-priced pizza |
| Q4 | Identify the most common pizza size ordered |
| Q5 | List the top 5 most ordered pizza types along with their quantities |

### 🟠 Intermediate (Q6–Q10)

| # | Question |
|---|----------|
| Q6 | Total quantity of each pizza category ordered |
| Q7 | Distribution of orders by hour of the day |
| Q8 | Category-wise distribution of pizzas |
| Q9 | Average number of pizzas ordered per day |
| Q10 | Top 3 most ordered pizza types based on revenue |

### 🟣 Advanced (Q11–Q13)

| # | Question |
|---|----------|
| Q11 | Percentage contribution of each pizza category to total revenue |
| Q12 | Cumulative revenue generated over time |
| Q13 | Top 3 most ordered pizza types by revenue for each category |

---

## 🛠️ Tools & Technologies

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)

- **Database:** MySQL
- **Tool:** MySQL Workbench
- **Concepts Used:**
  - Aggregate Functions (SUM, COUNT, AVG, ROUND)
  - JOINs (INNER JOIN across multiple tables)
  - Subqueries & Nested Queries
  - GROUP BY, ORDER BY, LIMIT
  - Window Functions (RANK, SUM OVER, PARTITION BY)
  - Date/Time Functions (HOUR)

---

## 🚀 How to Run

1. **Clone this repository**
   ```bash
   git clone https://github.com/8859384101/pizza-sales-sql.git
   cd pizza-sales-sql
   ```

2. **Import the dataset** into MySQL Workbench (orders, order_details, pizzas, pizza_types tables)

3. **Run queries** from the `queries/` folder in order:
   - Start with `basic_queries.sql`
   - Then `intermediate_queries.sql`
   - Finally `advanced_queries.sql`

---

## 📬 Connect with Me

[![GitHub](https://img.shields.io/badge/GitHub-8859384101-181717?style=for-the-badge&logo=github)](https://github.com/8859384101)

---

*Made with ❤️ and 🍕*
