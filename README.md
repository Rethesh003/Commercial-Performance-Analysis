#Commercial Performance Analysis
Overview:

This project analyzes 10,000 rows of American Superstore Sales data (2022–2023) .
The dataset was cleaned using Python (Pandas & NumPy), transformed with SQL & DAX, and visualized in Power BI.
It provides business insights across Sales, Profit, Customers, Discounts, Regions, and Products.

 Methodology (Step by Step):
1. Data Cleaning (Python – Pandas, NumPy)
Removed duplicates & null values.

Converted text dates into YYYY-MM-DD format.

Normalized column names (snake_case).

Created new derived columns like:

discounted_price = list_price × (1 – discount%)

profit = total_sales – total_cost

2. ETL & SQL Queries
Imported cleaned CSV into database.

Monthly sales & profit trend

Top products & categories

Statewise & city sales

Discount vs profit impact

Customer retention & repeat purchase rate

3. DAX (Power BI)
Created measures for better insights:

Profit Margin % = SUM(Profit) / SUM(Sales)

Avg Order Value = SUM(Sales) / DISTINCTCOUNT(Order_Id)

Retention Rate % = Returning Customers / Total Customers

Avg Items per Order = SUM(Quantity) / DISTINCTCOUNT(Order_Id)

4. Visualization (Power BI)
Designed an interactive dashboard with:

KPI cards (Sales, Profit, Orders, AOV, Profit %)

Line charts (Monthly Trends)

Bar/Tree maps (Category, State, City insights)

Donut charts (Customer segmentation)

Scatter plots (Discount vs Profit)

Added slicers for Year, Category, Customer Type, Region.

Tech Stack:
Python → Pandas, NumPy (data cleaning & preprocessing)

SQL → Data transformation & aggregation (20 queries)

DAX (Power BI) → Custom measures & KPIs

Power BI Desktop → Dashboard creation & storytelling

GitHub → Portfolio hosting

📂 Project Structure:
Commercial Performance Analysis
│── Dataset/cleaned_ecommerce_sales.csv   # Cleaned dataset (10K rows, 2022–2023)
│── Queries/SQL_Queries.sql               # 20 queries used for insights
│── PowerBI_Dashboard.pbix                # Final interactive Power BI dashboard
│── Screenshot 2025-09-24 120329.png      # Dashboard snapshots
│── README.md                             # Documentation

Dashboard Highlights
✔ KPI Cards → Total Sales, Profit, Orders, Avg Order Value, Profit Margin %
✔ Monthly Trends → Sales & Profit trends (2022–2023)
✔ Regional Insights → Sales & Profit by Region, State, City
✔ Customer Analysis → New vs Returning, Retention Rate, Avg Items/Order
✔ Product Insights → Sales by Category & Subcategory, Top Products
✔ Discount Impact → Profitability vs Discounts
✔ Shipping Mode Efficiency → Delivery method comparison

Key Insights:
1. Sales by Product Category & City wise:
Technology products perform best in Chicago (highest sales)
Whereas Furniture struggles in Springfield (lowest sales)
Recommendation: Focus marketing in Springfield and boost Furniture sales with targeted promotions.

2. Monthly Profit Trends:
 Both years (2022 and 2023) show October as the most profitable month (> ₹50,000 profit).
Recommendation: Use October seasonality to plan festive sales  campaigns and bulk promotions.

3. Shipment Mode Performance:
Standard Class shipping is the most used among the shipments it has 10 % profit but Second class contributes 10.58% profit, showing strong efficiency.
Recommendation: Continue leveraging Standard Class shipping but optimize costs in other modes.

4. Customer Retention & Growth:
 More than 90 % orders from old customers,Only 21 orders came from new customers.
 Recommendation: Launch discounts & loyalty offers to improve new customer acquisition.

5. Product Performance:
Top-selling: TEC-CO (Tech → Copies)
Second: OFF-BI (Office → Binders)
Third: TEC-MAC (Tech → Machines).
Recommendation: Stock more high-demand items (TEC-CO, OFF-BI), bundle with slower-moving items.

6.Regional Insights:
West region contributes 40% of sales with highest profit margin
Recommendation: Expand sales in wider like all regions to increase overall profit.





