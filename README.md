Pizza Sales Analytics Dashboard

##  Project Overview
An interactive 3-page Power BI dashboard designed to analyze retail pizza sales data, track top/bottom performing products, and provide dynamic breakdowns by pizza category and size.

##  Key Features & Pages
1. Pizza Sales Overview
2. Pizza Product Performance
3. Category & Size Analysis

##  Key SQL Queries Used for KPI Verification
### 1. Total Revenue
       select CAST(sum(total_price) AS DECIMAL(10,2)) as total_revenue
       from pizza_sales;

### 2. Total Orders Placed
       select count(distinct order_id) as total_Order
       from pizza_sales;

### 3. Total Pizza Sold
       select sum(quantity) as total_sold
       from pizza_sales;

### 4. Average Pizza Per Order
      select sum(quantity) / count(distinct order_id) as Average_pizza_per_order
      from pizza_sales;

### 5. Average Order Value
      select sum(total_price) / count(distinct order_id) as AOV
      from pizza_sales;

##  Dashboard Preview

### Page 1: Sales Overview
<img width="1322" height="731" alt="Page1 - Sales Overview" src="https://github.com/user-attachments/assets/c64abe26-d723-4d5d-a787-887bc6a6b190" />

### Page 2: Product Performance
<img width="1332" height="731" alt="Page 2 - Product Performance" src="https://github.com/user-attachments/assets/891341a9-c203-4bed-a95e-258aaa9b8c60" />

### Page 3: Category & Size Analysis
<img width="1324" height="726" alt="Page 3 - Category   Size Ananlysis" src="https://github.com/user-attachments/assets/f0b593cd-e20f-4795-8b69-06ac4be5e886" />

## 🛠️ Tools Used

* Power BI Desktopn: (Dashboard design, data modeling and DAX calculation)
* SQL(Structured Query Language): Data extraction, cleaning and querying database.
* Excel / CSV: (Raw transaction data source)

