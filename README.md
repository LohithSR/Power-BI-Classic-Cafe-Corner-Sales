# Power-BI-Classic-Cafe-Corner-Sales

Power BI Dashboard analyzing sales data of a Classic Cafe

# Project Title:

Classic Cafe Corner Sales Analysis (Power BI Dashboard)

# Introduction:

This project involves a sales data analysis of the Classic Cafe Corner using Power BI. The goal is to provide insights into key performance indicators (KPIs) such as total sales, profit margins, customer demographics, and product performance. The dashboard visualizes data in an interactive and intuitive way, offering decision-making insights.

## Dashboard Overview

Below is the dashboard's main page, displaying key sales performance metrics:

<img width="948" alt="Sales Dashboard Overview" src="https://github.com/user-attachments/assets/58b5e3d0-3f6f-40f9-8b0a-3d03cc1da5b5">

# Key Features:

Dashboard Overview: Provides a summary of cafe performance through KPIs like total revenue, average order value, customer satisfaction, and more.

Time-based Analysis: Breakdown of sales over time to identify peak periods and trends.

Customer Segmentation: Insights into customer demographics and purchasing behavior.

Product Performance: Identifies top-selling products and those with the highest profit margins.

# KPIs Tracked:

Total Sales

Number of Orders

Customer Satisfaction Score

Revenue per Customer

Product Sales Volume

## SQL Queries Used

### Data Preparation:

The following SQL queries were used to clean and transform the coffee shop sales data before importing it into Power BI for analysis.

**Convert Date and Time Columns:**

```sql
UPDATE coffee_shop_sales
SET transaction_date = STR_TO_DATE(transaction_date, '%d-%m-%Y');
```

**Total Sales Calculation:**

```sql
SELECT ROUND(SUM(unit_price * transaction_qty)) AS Total_Sales
FROM coffee_shop_sales
WHERE MONTH(transaction_date) = 5;
```

**Sales By Product Category:**

```sql
SELECT product_category, 
ROUND(SUM(unit_price * transaction_qty), 1) AS Total_Sales
FROM coffee_shop_sales
WHERE MONTH(transaction_date) = 5
GROUP BY product_category;
```

**Complete SQL Queries**:

[Download SQL Queries](https://github.com/user-attachments/files/17367352/MY.SQL.Queries.docx.pdf)


### Example of KPI Section:

<img width="952" alt="KPI Section" src="https://github.com/user-attachments/assets/ee7ce182-2d85-47f8-9a02-1a4578cd2591">


## Data Insights and Questions Answered

1. **Top Revenue-Generating Products:
   
   <img width="959" alt="Top Product " src="https://github.com/user-attachments/assets/c273f235-1196-4b7c-8171-f2c806d7c98c">

   - Breakdown of product sales performance.
   
3. **Monthly Sales Trends:**
   
  <img width="959" alt="Monthly Sales and Total Sales by Weekend" src="https://github.com/user-attachments/assets/8f11622d-2994-499c-a6a9-3a1684df9d91">

   - Insights on peak sales periods.

# Data Insights and Questions Answered:

What are the cafe's highest revenue-generating products?

During which months does the cafe experience the highest sales?

What is the average order value per customer?

How do sales differ across various customer demographics?

# Tools Used:

Power BI: For creating interactive dashboards and reports.

Data Source: [Coffee Shop Sales.xlsx](https://github.com/user-attachments/files/17366932/Coffee.Shop.Sales.xlsx)

# How to View the Dashboard:

Download the .pbix file from the repository.

Open it in Power BI Desktop to explore the visuals and interact with the data.

# Conclusion:

This Power BI project offers deep insights into sales performance, customer preferences, and product popularity, which are critical for improving the cafe's operational efficiency and decision-making. 

Key takeaways include:

Actionable Insights: The dashboard allows stakeholders to easily identify top-selling products and peak sales periods, enabling them to make data-driven decisions such as stocking inventory efficiently and focusing on high-demand products.

Data-Driven Decision Making: The analysis highlights trends over time and provides a clear understanding of customer behavior, helping the cafe tailor marketing strategies and promotions to specific customer segments.

Improved Business Strategy: By visualizing KPIs like revenue per customer and sales by product, the cafe can strategically focus on improving low-performing areas and enhancing customer satisfaction.

Scalability of the Model: This dashboard model can be extended to other cafe locations or expanded with additional data points like online sales, customer feedback, and supplier performance, offering a comprehensive view of the business as it grows.

Future Enhancements: In future iterations, more advanced analytics like forecasting sales, customer segmentation using machine learning, and incorporating more real-time data sources could further enhance decision-making.

This project showcases how leveraging data visualization tools like Power BI can transform raw data into valuable business insights, supporting the cafe’s goal of continuous growth and operational excellence.

## Contact

Feel free to reach out if you have any questions or would like to discuss this project further. I'm always open to networking opportunities and collaboration.

- **LinkedIn**: [Lohith S R](https://www.linkedin.com/in/lohith-s-r/)
- **GitHub**: [Lohith S R](https://github.com/LohithSR)
- **Email**: lohithmagnate2004@gmail.com

#
Thank you for reviewing my project! I look forward to connecting with you.


