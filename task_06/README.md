#  Online Sales Data Analysis – Project Summary

This project involves analyzing a transactional dataset from an online retail platform. The objective is to gain meaningful insights into product performance, revenue generation, and customer purchasing patterns using SQL-based queries executed in **MySQL Workbench**.

---

##  Dataset Description

The dataset, named `online_sales_data`, records individual sales transactions and contains the following key attributes:

- **Transaction_ID**: A unique identifier for each transaction  
- **Date**: The date when the transaction occurred (in DD-MM-YYYY format)  
- **Product_Category**: The category to which the purchased product belongs  
- **Product_Name**: Name of the product sold  
- **Units_Sold**: Number of units purchased in the transaction  
- **Unit_Price**: Price per unit (noted using comma as decimal)  
- **Total_Revenue**: Total revenue generated from the transaction  
- **Region**: Geographic location where the sale was made  
- **Payment_Method**: Mode of payment used by the customer  

---

##  Analysis Objectives

The analysis is structured to answer key business questions about sales performance and customer behavior, including:

1. **Identifying Monthly Patterns**  
   By extracting the month from the transaction date, we analyze how sales and revenue fluctuate across months.

2. **Tracking Monthly Revenue**  
   Summing revenue figures per month helps us understand peak sales periods and assess business performance over time.

3. **Evaluating Transaction Volume**  
   Counting the number of distinct transactions per month allows us to track customer activity and purchasing frequency.

4. **Regional Revenue Distribution**  
   Analyzing total revenue grouped by region provides insights into which geographic areas contribute the most to sales, guiding marketing and logistics decisions.

5. **Top-Selling Product Identification**  
   Determining the most popular product based on units sold highlights what customers prefer and can guide inventory planning.

6. **Revenue Contribution by Product Category**  
   Tracking how different product categories perform over time helps in understanding demand trends and seasonality.

---

##  Tools & Techniques

- **MySQL Workbench** for executing and testing SQL queries  
- Use of date functions for time-based grouping  
- Aggregation functions for revenue and volume metrics  
- Data cleaning techniques to handle string-formatted numerical fields

---

##  Business Insights Derived

- **Seasonal Trends**: Certain months consistently show higher revenue and transaction volumes, indicating seasonality.
- **Regional Dominance**: Some regions outperform others, helping prioritize regional promotions.
- **Product Preferences**: A few products and categories dominate sales, guiding stocking and marketing strategies.
- **Revenue Drivers**: High-value items contribute significantly to total revenue even with fewer units sold.

---

##  Report Documentation

The full analysis is compiled into a PDF report including:
- Detailed explanation of all queries used  
- Tabular results and screenshots  
- Business interpretations of each query result  
- Optional visualizations to support insights

---

##  Conclusion

This project demonstrates how structured SQL queries on transactional sales data can uncover actionable business insights. It forms a strong foundation for more advanced analytics such as customer segmentation, profitability analysis, and forecasting in the future.

---
