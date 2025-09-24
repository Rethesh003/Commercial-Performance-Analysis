# SPOC- (Sales-Profit-Order-Customer)Analysis
📌 Overview

This project analyzes 10,000 rows of American Superstore Sales data (2022–2023) .
The dataset was cleaned using Python (Pandas & NumPy), transformed with SQL & DAX, and visualized in Power BI.
It provides business insights across Sales, Profit, Customers, Discounts, Regions, and Products.

🚀 Methodology (Step by Step)

🔹 1. Data Cleaning (Python – Pandas, NumPy)
Removed duplicates & null values.

Converted text dates into YYYY-MM-DD format.

Normalized column names (snake_case).

Created new derived columns like:

discounted_price = list_price × (1 – discount%)

profit = total_sales – total_cost

🔹 2. ETL & SQL Queries
Imported cleaned CSV into database.

Monthly sales & profit trend

Top products & categories

Statewise & city sales

Discount vs profit impact

Customer retention & repeat purchase rate

🔹 3. DAX (Power BI)
Created measures for better insights:

Profit Margin % = SUM(Profit) / SUM(Sales)

Avg Order Value = SUM(Sales) / DISTINCTCOUNT(Order_Id)

Retention Rate % = Returning Customers / Total Customers

Avg Items per Order = SUM(Quantity) / DISTINCTCOUNT(Order_Id)

🔹 4. Visualization (Power BI)
Designed an interactive dashboard with:

KPI cards (Sales, Profit, Orders, AOV, Profit %)

Line charts (Monthly Trends)

Bar/Tree maps (Category, State, City insights)

Donut charts (Customer segmentation)

Scatter plots (Discount vs Profit)

Added slicers for Year, Category, Customer Type, Region.

🛠 Tech Stack
Python → Pandas, NumPy (data cleaning & preprocessing)

SQL → Data transformation & aggregation (20 queries)

DAX (Power BI) → Custom measures & KPIs

Power BI Desktop → Dashboard creation & storytelling

GitHub → Portfolio hosting

📂 Project Structure
Sales_Analysis/
│── Dataset/cleaned_ecommerce_sales.csv   # Cleaned dataset (10K rows, 2022–2023)
│── Queries/SQL_Queries.sql               # 20 queries used for insights
│── PowerBI_Dashboard.pbix                # Final interactive Power BI dashboard
│── Screenshots/                          # Dashboard snapshots
│── README.md                             # Documentation

📸 Dashboard Highlights
✔ KPI Cards → Total Sales, Profit, Orders, Avg Order Value, Profit Margin %
✔ Monthly Trends → Sales & Profit trends (2022–2023)
✔ Regional Insights → Sales & Profit by Region, State, City
✔ Customer Analysis → New vs Returning, Retention Rate, Avg Items/Order
✔ Product Insights → Sales by Category & Subcategory, Top Products
✔ Discount Impact → Profitability vs Discounts
✔ Shipping Mode Efficiency → Delivery method comparison

📊 Key Insights

Technology leads sales, while Furniture has low margins.

High discounts (>3%) directly reduce profit.

Standard Class shipping is most used, but Same Day is least profitable.

2023 saw 12% higher sales compared to 2022.

New customer is weak → 99% customers are old ones (returning buyers).


