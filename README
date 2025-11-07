🍫 Awesome Chocolates Sales & Shipment Analysis — End-to-End Power BI Project
📘 Project Overview

This project demonstrates an end-to-end Business Intelligence workflow, starting from data extraction using SQL, through data transformation with Power Query, and finally to data visualization in Power BI.

The goal of this analysis was to explore sales and shipment data for “Awesome Chocolates” and uncover insights related to total sales, profit margins, and performance by region, product, and category.

🧩 Project Objectives

Understand overall sales performance and profitability trends.

Identify top-performing regions, products, and sales reps.

Track shipment efficiency and order distribution.

Build an interactive Power BI dashboard that supports data-driven decision-making.

🛠 Tools & Technologies Used

SQL Server – for data extraction and cleaning.

Power Query (in Power BI) – for data transformation and preprocessing.

DAX (Data Analysis Expressions) – for creating KPIs and calculated measures.

Power BI Desktop – for data modeling and dashboard design.

🧹 Data Cleaning & Transformation Process

Imported raw sales and shipment data into SQL Server.

Cleaned and standardized data using SQL queries — removed nulls, duplicates, and formatting errors.

Loaded data into Power BI via Power Query and performed transformations:

Merged datasets (Sales, Regions, Products).

Applied filters for valid entries.

Created custom columns for profit, sales ratio, and shipment delay metrics.

🔢 Data Modeling

Defined relationships between tables (Sales ↔ Products ↔ Regions).

Added hierarchies for easier drill-down (Region → Country → Sales Rep).

Created calculated measures such as:

Total Sales = SUM(Sales[SalesAmount])

Profit Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[SalesAmount]))

Total Shipments = COUNT(Sales[OrderID])

📊 Dashboard Design & Visuals

The Power BI dashboard was designed for clarity, interactivity, and business storytelling.

Main Visual Components:

📈 KPI Cards – Total Sales, Profit Margin, Total Orders

🧭 Bar Chart – Region-wise sales distribution

🍩 Donut Chart – Category-wise revenue contribution

🕒 Line Chart – Sales trend over time

🧍‍♂️ Top 6 Performers Chart – Identifying high-performing sales reps

🎛 Slicers & Filters – Region, Product Category, Shipment Type

💡 Key Insights

Total Sales reached 141.49M, maintaining a 57.3% Profit Margin.

North Region contributed the highest to total revenue.

“Chocolate Bites” and “Milk Delight” were top-selling products.

Shipment delays were minimal, indicating operational efficiency.

📚 Learnings & Takeaways

Strengthened understanding of SQL-based data extraction and Power Query transformations.

Enhanced skills in data modeling, relationship management, and DAX calculation.

Learned to design visually balanced and business-oriented dashboards.

Improved ability to translate raw data into actionable insights for decision-making.

🧠 How SQL Was Used

I began the project by connecting the Power BI environment to a SQL Server database that stored raw shipment data. Using SQL queries, I:

Extracted shipment details from multiple related tables (Shipments, Products, Salespersons, Regions).

Performed initial data cleaning—removing nulls, handling duplicates, and standardizing product names.

Created aggregated tables for total sales and profit summaries by salesperson, region, and category.

Exported the cleaned dataset to Power BI for visualization.

Sample SQL Snippet:

SELECT 
    s.Salesperson,
    p.ProductName,
    r.Region,
    SUM(s.Boxes) AS TotalBoxes,
    SUM(s.Amount) AS TotalAmount,
    SUM(s.Profit) AS TotalProfit
FROM Sales s
JOIN Product p ON s.ProductID = p.ProductID
JOIN Region r ON s.RegionID = r.RegionID
GROUP BY s.Salesperson, p.ProductName, r.Region
ORDER BY TotalProfit DESC;


This SQL backbone ensured that my Power BI dashboard had accurate and pre-cleaned data, reducing transformation workload inside Power BI.

🪄 DAX Magic (In Power BI)

After loading the data, I used DAX (Data Analysis Expressions) to create calculated metrics like:

Total Amount = SUM(Sales[Amount])
Total Profit = SUM(Sales[Profit])
Profit % = DIVIDE([Total Profit], [Total Amount])
CY Amount = CALCULATE([Total Amount], YEAR(Sales[Date]) = 2025)
PY Amount = CALCULATE([Total Amount], YEAR(Sales[Date]) = 2024)
Growth % = DIVIDE([CY Amount] - [PY Amount], [PY Amount])


These formulas helped me design KPIs for sales growth, profitability, and year-over-year trends — giving the dashboard that real “corporate analytics” edge.

🧾 License

This project is open-sourced under the MIT License — feel free to explore, learn, and adapt the design.

❤️ Acknowledgement

This dashboard was crafted with deep curiosity, caffeine, and a love for turning data into stories.
Special thanks to the entire Power BI community for inspiring endless creativity.

🙌 About the Creator

This project was designed and developed by Mr. Srikanth, an aspiring analytics professional passionate about data visualization, storytelling, and business insights.

“Each end-to-end project I build brings me closer to mastering the art of transforming data into meaningful decisions.”
