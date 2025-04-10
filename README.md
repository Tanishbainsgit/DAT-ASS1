# DAT-ASS1

Business DB - Todd Cochrane
This project sets up a sample relational database system for a small business scenario. The database, business_db_todd_cochrane, manages customers, vendors, products, orders, and order items. It also includes various queries and views to demonstrate SQL functionalities such as joins, aggregations, filtering, and view creation.
Technologies Used
•	Microsoft SQL Server
•	T-SQL (Transact-SQL)

Database Structure
Tables
•	Customer: Stores customer details.
•	Vendor: Stores vendor information.
•	Product: Stores product listings associated with vendors.
•	OrderEntry: Represents customer orders.
•	OrderItem: Lists items within each order.
Relationships
•	Product → Vendor (many-to-one)
•	OrderEntry → Customer (many-to-one)
•	OrderItem → OrderEntry and Product (many-to-one)

Features
Database Initialization
•	Forces disconnect and drops the database if it exists.
•	Creates the database and tables with constraints.
•	Inserts sample data for vendors, products, customers, and orders.
Queries
1.	Products Not Made by DLL01
2.	Products Priced Between $5.00 and $10.00
3.	Products by Specific Vendors (≥ $10.00)
4.	Average Product Price
5.	Total Number of Customers
6.	Customers with Non-empty Email Addresses
7.	Product Count + Min, Max, Avg Price
8.	Product & Vendor Information
9.	Order #20007 Details
10.	Customers Who Ordered Product 'RGAN01'
11.	Orders Placed by Customer (Grouped by Name and City)
12.	Targeted Customers (City or Name-Based Filter)
Views
•	vProductCustomer: Links customers to products through orders.
•	vCustomerMailingLabel: Formats a customer mailing label (including incomplete addresses).
•	vCustomerMailingLabel_Valid: Filters for only complete mailing addresses.
How to Use
1.	Open SQL Server Management Studio (SSMS).
2.	Run the entire script in a new query window.
3.	Ensure you're connected to a server with appropriate permissions to:
o	Create and drop databases.
o	Insert data and create views.

