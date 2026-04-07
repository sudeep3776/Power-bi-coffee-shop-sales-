# Power-bi-coffee-shop-sales-

 ## Project Title
 
Coffee Shop Sales Analytics Dashboard | Power BI Business Intelligence Project

# Dataset used 
- <a href="https://github.com/sudeep3776/Power-bi-coffee-shop-sales-/blob/main/Coffee%20Shop%20Sales.xlsx"> Dataset view
- <a href="https://github.com/sudeep3776/Power-bi-coffee-shop-sales-/blob/main/Coffee%20shop%20sales%20DashBoard.pbix"> Dashboard view</a>


 ## Overview
 
This project delivers a single-page, fully interactive Power BI dashboard for a multi-location coffee shop chain. It connects to a structured transactions dataset, applies custom DAX measures, and visualizes business performance across four key dimensions:

Time — Sales by day, hour, week, and month
Location — Revenue comparison across store locations
Product — Category and product-type level sales breakdown
Customer Behaviour — Weekday vs. weekend patterns and peak hour analysis

The dashboard features custom tooltips (calendar chart tooltip, day & hour tooltip), a dynamic filter panel (Month slicer), and KPI cards for real-time summary metrics — all styled in a dark coffee-themed UI.

##  Problem Statement
 
Coffee shop owners and managers often operate without clear visibility into:

When their peak sales hours and days actually occur
Which products and categories drive the most revenue
How individual store locations compare against each other
Whether weekday or weekend traffic generates more revenue
Month-over-month growth — are sales improving or declining?

Without structured reporting, decisions on staffing, inventory, promotions, and store expansion rely on intuition. This dashboard replaces guesswork with data.

 Dataset



##  Tools & Technologies
 
ToolPurposePower BI DesktopDashboard design, data modeling, DAX, publishingDAX (Data Analysis Expressions)Custom measures — Total Sales, MoM Growth, Placeholder logic, TooltipsPower Query (M Language)Data transformation and loadingMicrosoft Excel (.xlsx)Source data filePower BI Date TableCustom date dimension for time intelligencePower BI TooltipsCustom tooltip pages for calendar and hourly chart drill-through


##  Methodd

### Data Loading & Transformation

### Data Modeling

### DaX Measures Created
DAXTotal Sales       = SUM(Transactions[transaction_qty] * Transactions[unit_price])

Total Orders      = COUNTROWS(Transactions)

Total Quantity    = SUM(Transactions[transaction_qty])

MoM Growth        = (Current Month Sales - Previous Month Sales) / Previous Month Sales

### Dashboard Design

Built 3 report pages: Main Dashboard, Tooltip (Calendar), Tooltip (Day & Hour)
Applied dark coffee-themed color palette (#36003E header, #402B1E panels)
Used custom background image and coffee cup branding for professional polish
Built a pivot table heatmap for Hour × Day of Week sales matrix

### Interactivity & Filtering

Month slicer for period-level filtering
Cross-filtering enabled across all visuals
Custom tooltip pages embedded on Calendar Chart and Day/Hour chart


##  Key Insights

Sales trend over time — The column chart reveals clear monthly sales peaks and troughs, identifying seasonal patterns in coffee shop revenue

Weekday vs. Weekend split — The donut chart shows whether the coffee shop is a commuter-driven business (weekday-heavy) or a leisure destination (weekend-heavy) — critical for staffing decisions

Peak Hours identified — The Hour × Day heatmap (pivot table) and bar chart pinpoint the exact hours driving maximum revenue — typically morning rush (7–10 AM) for coffee shops

Store Location comparison — The clustered bar chart compares Total Sales across all store locations, instantly highlighting the best and worst performing outlets

Product Category leaders — The horizontal bar chart ranks product categories (e.g., Coffee, Tea, Bakery, Drinking Chocolate) by revenue contribution

Product Type deep-dive — A second product-level chart breaks performance down further by specific product types within each category

MoM Growth tracking — The tooltip layer surfaces Month-over-Month growth percentage on hover, enabling quick trend assessment without cluttering the main view

Calendar heatmap — The custom tooltip on the calendar view shows daily Sales, Orders, and Quantity Sold — making it easy to spot individual high-revenue days


##  Dashboard / Output
 Screenshot <img width="1457" height="882" alt="Screenshot dashboard" src="https://github.com/user-attachments/assets/79b3ab5c-dab0-46f5-951e-759edff029ed" />


Shows: Total Sales, Total Orders, Total Quantity, MoM Growth on hover over calendar dates

Tooltip Page 2 — Tool Tip - Day & Hour chart

Shows: Total Sales, Total Orders, Total Quantity, MoM Growth on hover over day/hour visuals

File: Coffee_shop_sales_DashBoard.pbix
