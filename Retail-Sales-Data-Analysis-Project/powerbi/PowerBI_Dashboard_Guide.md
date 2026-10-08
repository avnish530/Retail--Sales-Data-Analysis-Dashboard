# Power BI Dashboard Guide
1. Open Power BI Desktop.
2. Get Data -> Text/CSV -> select data/retail_sales_cleaned.csv.
3. Create measures:
Total Sales = SUM(retail_sales_cleaned[Sales])
Total Profit = SUM(retail_sales_cleaned[Profit])
Total Orders = DISTINCTCOUNT(retail_sales_cleaned[Order_ID])
Total Quantity = SUM(retail_sales_cleaned[Quantity])
Average Order Value = DIVIDE([Total Sales],[Total Orders])
Profit Margin = DIVIDE([Total Profit],[Total Sales])

Recommended visuals:
- KPI Cards: Total Sales, Total Profit, Total Orders, Profit Margin
- Line chart: Sales by Order_Date/Month
- Bar chart: Sales by Region
- Column chart: Profit by Category
- Bar chart: Top 10 Products by Sales
- Table: Top Customers with Sales and Profit
- Slicers: Region, Category, Product, Order_Date
