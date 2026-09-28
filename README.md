# ONLINE-BOOK-STORE-ANALYSIS
SQL-based analysis of an online bookstore using books, customers, and order data to uncover sales, customer, inventory, and genre-level insights.
Online Book Store Analysis is a SQL-based data analysis project designed to analyze an online bookstore's books, customers, and orders.

The project uses SQL to explore book information, customer details, order transactions, sales, inventory, genres, and customer purchasing behavior.

The database contains three main tables:
Books
Customers
Orders

The Orders table connects customers with the books they purchase using foreign-key relationships.

 Project Objectives:
Analyze bookstore inventory.
Explore different book genres.
Analyze customer information.
Examine customer orders.
Calculate total revenue.
Identify expensive and low-stock books.
Analyze book sales by genre.
Identify frequently ordered books.
Analyze customer spending.
Analyze sales by author.
Calculate remaining stock after fulfilling orders.

Database Structure

The project consists of three primary tables:

1.Books

The Books table contains information about books available in the bookstore.

Column	Description
Book_ID	Unique ID of the book
Title	Book title
Author	Author of the book
Genre	Genre/category of the book
Published_Year	Publication year
Price	Price of the book
Stock	Available stock

2. Customers

The Customers table contains customer information.

Column	Description
Customer_ID	Unique customer ID
Name	Customer name
Email	Customer email
Phone	Customer phone number
City	Customer city
Country	Customer country

3.  Orders

The Orders table contains bookstore transaction information.

Column	Description
Order_ID	Unique order ID
Customer_ID	ID of the customer
Book_ID	ID of the purchased book
Order_Date	Date of order
Quantity	Number of books ordered
Total_Amount	Total amount of the order

The Orders table uses relationships with both Customers and Books.

🔗 Database Relationship
Customers
    │
    │ Customer_ID
    ▼
  Orders
    │
    │ Book_ID
    ▼
  Books
Relationship
Customers 1 ──────────── * Orders * ──────────── 1 Books

A customer can place multiple orders, while a book can appear in multiple orders.

🔍 SQL Analysis

The project contains both basic SQL queries and advanced SQL analysis queries.

🟢 Basic SQL Queries

The analysis includes questions such as:

Retrieve all Fiction books.
Find books published after 1950.
Find customers from Canada.
Retrieve orders placed in November 2023.
Calculate total available stock.
Find the most expensive book.
Find orders where quantity is greater than 1.
Find orders with a total amount greater than $20.
Retrieve distinct book genres.
Find the book with the lowest stock.
Calculate total revenue.

These queries demonstrate fundamental SQL operations such as SELECT, WHERE, DISTINCT, filtering, aggregation, and sorting.

🔵 Advanced SQL Analysis

The project also contains more advanced analysis involving joins, grouping, aggregation, and customer-level analysis.

Advanced Questions
Calculate total books sold per genre.
Calculate the average price of Fantasy books.
Find customers who placed at least two orders.
Identify the most frequently ordered book.
Find the top three most expensive Fantasy books.
Calculate total quantity sold by each author.
Find cities where customers have spent more than $30.
Identify the customer who spent the most.
Calculate remaining stock after fulfilling orders.
