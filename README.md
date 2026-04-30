# customer_behavior_analysis
Data analytics project showcasing customer behavior analysis using Python ,SQL and Power Bi

# 🛒 Customer Shopping Behavior Analysis

An end-to-end data analytics portfolio project demonstrating data cleaning, database management, and interactive data visualization. This project analyzes customer shopping trends, demographic spending habits, and the impact of promotional discounts on product sales.

## 🛠️ Tech Stack & Tools
* **Data Wrangling:** Python (Pandas, Jupyter Notebook)
* **Database & Querying:** PostgreSQL (pgAdmin)
* **Data Visualization & Modeling:** Power BI
* **Version Control:** Git & GitHub

## 🎯 Project Objective
To extract actionable business insights from raw retail data by answering key questions:
1. Which customer demographics (e.g., gender, age) drive the highest revenue?
2. What are the most popular product categories?
3. Which specific products have the highest percentage of discount-driven purchases?

## 🚀 Workflow (The 6 Steps)

### 1. Data Sourcing & Definition
* Sourced the `customer_shopping_behavior.csv` dataset containing exactly 3,900 customer records.
* Defined key KPIs and business questions to guide the analytical approach.

### 2. Data Cleaning (Python)
* Imported raw data into a Jupyter Notebook using the `pandas` library.
* Standardized column names (e.g., transforming "Discount Applied" to `Discount_Applied` for SQL compatibility).
* Handled missing values and removed duplicate records to ensure data integrity.
* Exported the clean dataset for database ingestion.

### 3. Database Storage & Exploratory SQL (PostgreSQL)
* Created a relational schema and loaded the cleaned CSV into a local PostgreSQL database.
* Conducted Exploratory Data Analysis (EDA) using SQL.
* **Sample Query:** Used a `CASE` statement and subqueries to calculate the exact percentage of discounted purchases per item, revealing that items like Hats and Sneakers are highly discount-dependent.

### 4. Data Connection & Modeling (Power BI)
* Established a direct Import connection from Power BI Desktop to the local PostgreSQL server via `localhost`.
* Verified data types and configured the tabular data model.

### 5. Dashboard Visualization & UI
* Designed a custom, data-themed 16:9 background for a professional UI layout.
* Configured visuals with 100% transparency to seamlessly integrate with the background design.
* Built interactive Donut Charts (Gender distribution), Bar Charts (Item purchases), and KPI Cards (Total Customers, Average Purchase Amount).
* Customized Data Labels to display exact hard numbers (e.g., 2,652 Male vs. 1,248 Female) alongside percentages for absolute clarity.

### 6. Key Business Insights
* **Demographic Revenue:** Male customers account for exactly 68% of the customer base (2,652 vs 1,248) and proportionally drive higher overall purchase volume.
* **Discount Dependency:** Certain apparel items are highly reliant on promotions. For example, 50% of all Hats and 49.66% of Sneakers are bought *only* when a discount is applied.
* **Average Spend:** The average customer transaction hovers around $60.88, providing a baseline metric for future upselling or marketing campaigns.

---
*This project structure was inspired by the methodology outlined in Amlan Mohanty's 6-step analytics framework.*
