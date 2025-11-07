# MYSQL
🗄️ SQL Project – Sample Superstore Analysis
📘 Overview
This project demonstrates practical SQL queries and operations on the Sample Superstore dataset. It covers fundamental and intermediate SQL concepts including data retrieval, aggregation, filtering, joins, and functions, showcasing how SQL can be used for analytical insights.
The project follows the CRUD principle — Create, Read, Update, and Delete — and applies major SQL sublanguages such as DDL, DML, TCL, DCL, and DQL.

🧠 Learning Objectives


Understand and apply different SQL command categories:

DDL (Data Definition Language) – Create, Rename, Alter, Truncate, Drop
DML (Data Manipulation Language) – Insert, Update, Delete
TCL (Transaction Control Language) – Commit, Savepoint, Rollback
DCL (Data Control Language) – Grant, Revoke
DQL (Data Query Language) – Select, Projection, Selection, Joins

Practice querying techniques to extract insights from the Sample Superstore dataset.
Strengthen database management and query optimization skills.

🧩 Dataset
Table Name: samplesuperstore
This table includes columns such as:

City
State
Region
Country
Category
Sub-Category
Sales
rofit
Quantity
Discount
Segment
Customer Name

🧮 Key SQL Queries
Here are examples of the types of queries included in this project:
#DescriptionExample Query1Display city and stateSELECT city, state FROM samplesuperstore;2Show total salesSELECT SUM(sales) FROM samplesuperstore;3Sales from FloridaSELECT state, SUM(sales) FROM samplesuperstore WHERE state='Florida';4Profit > 150 with sub-categorySELECT sub_category, profit FROM samplesuperstore WHERE profit > 150;5Adjust sales ±25%SELECT sales*0.75 AS Deduction, sales*1.25 AS Hike FROM samplesuperstore;6Profit of city Fort LauderdaleSELECT city, profit FROM samplesuperstore WHERE city='Fort Lauderdale';7Sales by region and countrySELECT region, country, SUM(sales) FROM samplesuperstore GROUP BY region, country;8Quantity sold by stateSELECT state, SUM(quantity) FROM samplesuperstore GROUP BY state;9Average discount by segmentSELECT segment, AVG(discount) FROM samplesuperstore GROUP BY segment;10Average salesSELECT AVG(sales) FROM samplesuperstore;...(Additional queries 11–20 for advanced analytics)—

🧰 Tools Used
MySQL Workbench / phpMyAdmin
SQL CLI or GUI

Sample Superstore Dataset
⚙️ Setup Instructions

Install MySQL.

Create a database:
CREATE DATABASE samplesuperstore_db;
USE samplesuperstore_db;
Import the dataset and create the samplesuperstore table.
Run queries from the provided SQL script or .pdf file.

📈 Concepts Covered

CRUD Operations
Aggregate Functions
Group By and Having Clauses
Conditional Queries (WHERE, LIKE, BETWEEN)
String and Numeric Functions
Data Sorting and Filtering
Subqueries and Joins
Data Manipulation and Transactions

🧾 Author
K. Bhargavi
Project prepared as part of SQL learning and database analysis practice.

🏁 Conclusion
This MySQL project provides hands-on experience in data manipulation and analytics using SQL. By working with the Sample Superstore dataset, users can gain a strong understanding of SQL commands, query building, and database design principles.

