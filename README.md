XDTask 3 – SQL for Data Analysis

📌 Project Overview

This project was completed as part of the Data Analyst Internship – Task 3: SQL for Data Analysis.

The objective of this task was to use SQL queries to create, manipulate, and analyze structured e-commerce data.

🎯 Objective

The main objective of this task was to learn how to:

- Create and manage database tables
- Insert and work with structured data
- Retrieve data using SQL queries
- Filter and sort data
- Group and summarize data
- Use aggregate functions
- Perform table joins
- Use subqueries
- Create views for analysis
- Handle NULL values
- Improve query performance using indexes

🛠️ Tools Used

- SQL
- Online SQL Editor
- MySQL-compatible SQL syntax
- GitHub

📊 Database

The project uses a sample E-commerce database consisting of four tables:

1. Customers

Stores customer information.

Columns:

- "customer_id" – Unique customer ID
- "name" – Customer name
- "email" – Customer email
- "signup_date" – Customer registration date

2. Products

Stores product information.

Columns:

- "product_id" – Unique product ID
- "product_name" – Name of the product
- "category" – Product category
- "price" – Product price

3. Orders

Stores customer order information.

Columns:

- "order_id" – Unique order ID
- "customer_id" – ID of the customer who placed the order
- "order_date" – Date of the order

4. OrderItems

Stores individual products included in each order.

Columns:

- "item_id" – Unique item ID
- "order_id" – Related order ID
- "product_id" – Related product ID
- "quantity" – Number of products purchased
- "unit_price" – Price per unit

🔗 Table Relationships

The database uses primary keys and foreign keys to connect the tables.

- "Orders.customer_id" → "Customers.customer_id"
- "OrderItems.order_id" → "Orders.order_id"
- "OrderItems.product_id" → "Products.product_id"

An index was also created on "Orders.customer_id" to help optimize queries involving customer IDs.

🗂️ Sample Data

The database contains sample data for:

- 4 customers
- 4 products
- 4 orders
- 5 order items

The sample data includes products from categories such as Electronics and Furniture.

🔍 SQL Concepts Covered

The following SQL concepts were practiced in this task:

Basic Queries

- SELECT
- WHERE
- ORDER BY
- GROUP BY

Aggregate Functions

- SUM()
- AVG()
- COUNT()

Joins

- INNER JOIN
- LEFT JOIN
- RIGHT JOIN

Advanced SQL

- Subqueries
- Views
- NULL value handling
- Indexes

⚡ Query Optimization

An index was created on the "customer_id" column of the "Orders" table:

CREATE INDEX idx_orders_customer_id ON Orders(customer_id);

This was done as part of the query optimization requirement.

The GitHub repository contains:

- "schema.sql" – Database tables, relationships, sample data, and index creation
- "queries.sql" – SQL queries used for data analysis
- "README.md" – Project documentation
- "queries 1 to 4/" – Screenshots showing SQL query outputs

Screenshots of the executed SQL queries and their outputs are included in the "queries 1 to 4" folder as evidence of the analysis performed.

📌 Learning Outcome

Through this task, I learned how to use SQL to create and work with structured databases, retrieve useful information, analyze e-commerce data, connect multiple tables using joins, use subqueries and views, and apply indexes for query optimization.

👩‍💻 Author

Sarthaki Narnaware

B.Tech – Electronics & Telecommunication Engineering


