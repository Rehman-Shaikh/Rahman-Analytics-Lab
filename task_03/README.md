# Rahman-Analytics-Lab

#  SQL Mini Guide using Shipments Dataset

This document explains how to analyze a shipments dataset using core SQL concepts. The dataset includes information like shipment mode, customer rating, product importance, and delivery status.

---

###  A. SELECT, WHERE, ORDER BY, GROUP BY

- **SELECT** is used to fetch data from a table. You can retrieve all or selected columns using this.
- **WHERE** helps filter records based on conditions, such as only showing high-priority products.
- **ORDER BY** sorts the result in ascending or descending order — for example, sorting by discount offered.
- **GROUP BY** is used to group rows that have the same values in specified columns and is often used with aggregate functions like COUNT, AVG, etc.

 *Example:*  
"Show average discount per shipment mode" → Use `GROUP BY Mode_of_Shipment`.

---

###  B. JOINS (INNER, LEFT, RIGHT)

JOINs are used to combine data from two tables based on a related column.
And here i have created a seprate table named 'customer_detail'
and it is having these data.
"
about 'gender'  and 'name' column only.
"

- **INNER JOIN** returns only the matching records in both tables.
- **LEFT JOIN** returns all records from the left table and matched records from the right.
- **RIGHT JOIN** is the opposite — it returns all records from the right and matched ones from the left.

Since our dataset has customer gender, we can create a dummy table `customer_details` with names and genders, then JOIN it with the `shipments` table on the `Gender` field to combine both datasets.

---

###  C. Subqueries

A subquery is a query inside another query.

You can use subqueries to:
- Compare values with averages or maximums
- Filter using results of another query

 *Example:*  
"Show only shipments where discount is higher than average" → Use subquery inside WHERE clause.

---

###  D. Aggregate Functions

These functions help summarize data:
- **SUM()** adds values
- **AVG()** finds average
- **COUNT()** counts rows
- **MIN() / MAX()** find lowest/highest

 *Example:*  
"Find total discount per warehouse" → Use `GROUP BY Warehouse_block` with `SUM()`.

---

###  E. Views

A **view** is like a saved query. It behaves like a virtual table that stores results of a SQL query.

Use views when:
- You want to frequently access filtered data (e.g., only on-time deliveries)
- You want to simplify complex queries

 *Example:*  
Create a view of all high-discount shipments and use it in future queries directly.

---

###  F. Indexes

**Indexes** improve performance of SQL queries by allowing faster search and filtering.

Use indexes when:
- You frequently use `WHERE`, `JOIN`, or `ORDER BY` on specific columns.
- You want to speed up filtering on columns like `Product_importance` or `Mode_of_Shipment`.

 *Note:* Indexes increase read performance but may slightly slow down insert/update speed.

---

###  Conclusion

This guide gives a hands-on introduction to:

- Querying and analyzing shipment data
- Combining tables with JOINs
- Using aggregate functions and subqueries
- Creating views for repeated queries
- Optimizing with indexes

You can now write smarter queries and perform detailed analysis on real-world data!


