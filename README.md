# Sales-Performance-Dashboard #
- An interactive Power BI dashboard that provides a complete view of sales performance. It tracks Sales, Profit, Quantity, Discounts, and highlights top-performing products, categories, and regions. Built with DAX measures, data modeling, and visualization best practices to deliver actionable business insights.
 ---
 
For this project, I applied the full data analysis process:
## 1️⃣ Descriptive Analytics:
•	Analyzed historical data to display key financial metrics like total sales, costs, and net profit, highlighting sales patterns by product, category, and geography.
## 2️⃣ Diagnostic Analytics:
•	Investigated the root causes of issues, such as low sales in specific markets (e.g., Denmark) and underperforming products like SanDisk. I used RFM segmentation to identify valuable and at-risk customers.
## 3️⃣ Predictive Analytics:
•	Used predictive modeling to forecast 2025 sales, identifying potential declines and emphasizing the need for proactive strategies to sustain growth.



---

![Main-Dashboard](https://github.com/user-attachments/assets/99fb59a2-1ea1-4b8d-becc-ed6ba5148211)

---

## 📑 Table of Contents
- [Project Overview](#-sales-analysis-dashboard)
- [📊 Key Features](#-key-features)
- [💡 Business Insights](#-business-insights)
- [🛠 Tools Used](#-tools-used)
- [🧹 Data Cleaning](#-data-cleaning)
- [🏗 Data Modeling](#-data-modeling)
- [🎯Business Questions](#-business-questions)



## 📊 Key Features
- **Total Sales, Cost, Profit & Gross Margin, Unique Customer, Unique Order, Trans AVG, and Total Quantity** tracking.
- **Overview Sales Analysis**: Total Sales and profit per year, Sales by many dimensions like sales by category and sub-category, country and city.
- **Product Overview** for Top-selling products and top 3 profitable products.
- **Products Analysis (Root Cause Analysis)** with know why year 2021 was the least year in total sales and 2024 was the biggest.
- **RMF Customer Segmantation** RFM Segmentation is a data-driven technique used to understand and categorize customers based on their.
- **Forecasting Analysis** the process of using historical data to predict future trends and performance.
In this project, forecasting techniques are applied to sales data to anticipate upcoming results and support decision-making..
- **Data Modelling&Data Cleaning** 

---

## 💡 Business Insights
- **1️⃣ Overall Sales Performance:** 
•	Total Sales: $2,35M
•	Total Cost: $2,06M
•	Net Profit: $283K
•	Gross Margin: 12.06%

- **2️⃣ Geographical Insights:**
•	France leads with $608K in sales, followed by Germany ($483K), and United kingdom ($418K).
•	London is the top-performing city, while Denmark shows very low sales with only $34 recorded.



![MainDashboard](https://github.com/user-attachments/assets/fd11377d-6449-47d4-b109-e727e29f7f91)

---
 
- **3️⃣ Product Performance:** 
•	Defining top 5 selling product ( Eldon file card is the top one  product selling) 
•	I used the biggest year of financial growth and was able to identify the products that contributed to this boost.



![Product Analysis](https://github.com/user-attachments/assets/23091a22-8585-44f7-a5f4-0e843dff3057)

---
 

- **4️⃣ Customer Segmentation (RFM Analysis):** 
•	104 Champions: These are the highest-value customers.
•	117 At-Risk customers: They represent a critical area for retention strategies.
•	New and Promising Customers show potential for future growth.



![RMF](https://github.com/user-attachments/assets/a11c35da-be53-4d34-a470-4d08b600e64f)

---
 

- **5️⃣ Sales Forecast for 2025:** 
•	Projected Sales: with total sales $2.34(from 2021 to 2024), emphasizing the need for proactive actions to sustain growth.


<img width="894" height="501" alt="Forecast" src="https://github.com/user-attachments/assets/efd5a617-24d3-4a21-9452-c0e4bc664b9e" />

---

## 🛠 Tools Used
- **• Power Bi**: Data Modelling, DAX, and Visualization.  
- **•	ETL & Data Cleaning**: using Power Query.  
- **•	Advanced Calculations**: using Data Analysis Expressions (DAX).
- **•	Snowflake Schema Modelling**: for scalable, efficient reporting.
- **•	RFM Segmentation**: for customer behaviour analysis.
- **•	Sales Forecasting & Scenario Analysis**: for future planning.


---

## 🧹 Data Cleaning
Performed in **Power Query Editor**:
- Removed duplicates and blank rows  
- Standardized column names  
- Handled missing data (imputation/removal where necessary)  
- Changed data types for consistency (dates, currency, integers)  
- Renamed and reordered columns for clarity  
- Created calculated columns (e.g., `SalesValue = OrderQuantity * UnitPrice`)
  
---

<img width="1166" height="555" alt="Fact clean" src="https://github.com/user-attachments/assets/43f8a860-859c-4c70-a563-9b1abce83611" />




![dim order clean](https://github.com/user-attachments/assets/f1e2f60d-2af8-46eb-adcd-b886584653e7)

---

## 🏗 Data Modeling
Designed a **Snowflake Schema** in Power Pivot with relationships between fact and dimension tables:

![9](https://github.com/user-attachments/assets/ec28a560-d66f-42d7-ac3f-26db53c87a28)


- **Fact Tables**: `Fact_sales` & `Fact RMF Customer Segmantion` 

- **Dimension Tables**: Customers, Products, Country, City, Ship mode, Orders, Category, and Sub-Category  

- **Dim-Callender**: I have built it using DAX

![Dim-Callendar](https://github.com/user-attachments/assets/6578d48a-8a6b-4923-9799-cfaa94626dc2)


- Built **primary–foreign key relationships** to enable robust analysis  

---

## Measures
- 01.Total Sales
- 02.Net Profit Value
- 03.Total Cost Of Product S0ld
- 04.Gross Margin(%)
- 05.Total Transactions
- 06.Unique Orders
- 07.Unique Customers
- 08.Transaction AVG.
- 09. AVG. of Cost Per Product
- 10.AVG Revenue Per Customer(ARPC)
- 11.Total Quantity
- 12.Fact Min Transaction
- 13.Fact Max Transaction
- 14. Sales Running Total(_RT)
- 15. Used Discount
- 16.New Customers
- 17.Last Timers
- 18.Repetative Customers
- 19.AVG Discount
- 20.Discount Amount
- 21.Free Goods
- 22.Num of products S0ld with discount
- 23.ROI
- 24.Unique Products
- 25.YoY %
  
### Forecasting Dax-FX
- Fx-1 2025 Total Cost Forecast
- Fx-2 2025 Total Profit Forecast
- Fx-3 Total Forecast
---

![10](https://github.com/user-attachments/assets/136034b1-2b54-4a1f-8ec3-1d516f88e28b)


![11](https://github.com/user-attachments/assets/750ea207-1770-48ad-ac3c-1a4ed466d8d1)



---

## 🎯 Business Questions

### 1. Descriptive Statistics:
• Mean, Median, Mode, and Standard Deviation of sales, profit, quantity, and discount. 
• Count of unique orders, products, categories, and sub-categories. 
• Distribution of sales and profit by category or sub-category. 
### 2. Time-Series Analysis: 
• Trends in sales and profit over time (using order date). 
• Seasonal patterns in sales and profit. 
• Monthly or yearly sales growth rates. 
### 3. Product Analysis: 
• Best-selling products (based on quantity sold or total sales). 
• Products with the highest profit margins. 
• Products with the most significant discounts. 
### 4. Category/Sub-Category Analysis: 
• Category or sub-category with the highest sales and profit. 
• Category or sub-category with the most significant discounts. 
• Growth trends for different categories. 
### 5. Discount Analysis: 
• Effect of discounts on sales and profit. 
• Calculate the discount rate distribution. 
• Identify if certain products or categories are more sensitive to discounts. 
### 6. Profitability Analysis: 
• Calculate the overall profit margin (total profit divided by total sales). 
• Profitability by product, category, or sub-category. 
• Identify products or categories with low profitability. 
### 7. Quantity Analysis: 
• Quantity sold for each product, category, or sub-category. 
• Quantity sold over time to identify trends. 
• Correlation between quantity sold and other variables (e.g., profit, discount). 
### 8. Order Analysis: 
• Average order value (total sales divided by the number of orders). 
• Distribution of order values. 
• Customer segmentation based on order size. 
### 9. Customer Analysis : 
• Customer segmentation based on purchase behavior. 
• Customer lifetime value (CLV) calculations. 
• Customer retention rate and churn analysis. 
### 10. Geographic Analysis: 
• Sales and profit by region or location. 
• Identify regions with the highest and lowest performance. 
### 11. Inventory Analysis : 
• Inventory turnover rate (how quickly products are sold). 
• Identify slow-moving or overstocked items. 
### 12. Forecasting : 
• Use time-series data to forecast future sales and profit. 
• Predict demand for specific products or categories



📌 With this analysis, business leaders can make **data-driven decisions** about product focus, regional strategy, and customer engagement.  
