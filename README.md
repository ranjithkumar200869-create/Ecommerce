# E-Commerce Database Management System

## 📌 Project Overview

The **E-Commerce Database Management System** is a database project designed to manage the major operations of an e-commerce business.

The system stores and manages information related to:

* Customers
* Products
* Orders
* Payments
* Sellers
* Reviews

The main goal is to maintain accurate, organized, and reliable e-commerce data using a relational database.

## 🎯 Objectives

The main objectives of this project are:

1. Store and manage customer information.
2. Store product details such as name, price, stock, and category.
3. Maintain customer orders and order details.
4. Store payment information for orders.
5. Maintain seller information.
6. Allow customers to provide product reviews and ratings.
7. Support CRUD operations for administrators.
8. Maintain data accuracy using database constraints.

## 🏢 Business Requirements

The system should provide the following functionalities:

* Customer registration and information management.
* Product information management.
* Order management.
* Payment management.
* Seller management.
* Product reviews and ratings.
* Administrative CRUD operations.
* Data integrity using primary keys, foreign keys, unique constraints, and other constraints.

## 🗂️ Database Entities

The system contains the following major entities:

| Entity   | Description                                          |
| -------- | ---------------------------------------------------- |
| Customer | Stores customer personal and contact information     |
| Product  | Stores information about products available for sale |
| Order    | Stores customer order information                    |
| Payment  | Stores payment details for orders                    |
| Seller   | Stores information about sellers                     |
| Review   | Stores customer reviews and ratings for products     |

## 🔗 Relationships

The main relationships in the system are:

* A **Customer** can place many **Orders**.
* An **Order** can contain multiple **Products**.
* A **Product** can be sold by a **Seller**.
* An **Order** can have a **Payment**.
* A **Customer** can write multiple **Reviews**.
* A **Product** can receive multiple **Reviews**.

## 👤 Customer Table

The Customer table stores customer personal and contact information.

| Attribute   | Data Type    | Constraint                  | Description           |
| ----------- | ------------ | --------------------------- | --------------------- |
| customer_id | INT          | PRIMARY KEY, AUTO_INCREMENT | Unique customer ID    |
| first_name  | VARCHAR(50)  | NOT NULL                    | Customer first name   |
| last_name   | VARCHAR(50)  | NOT NULL                    | Customer last name    |
| email       | VARCHAR(100) | UNIQUE, NOT NULL            | Customer email        |
| phone       | VARCHAR(15)  | UNIQUE                      | Customer phone number |
| address     | VARCHAR(255) | NOT NULL                    | Customer address      |
| city        | VARCHAR(50)  | NOT NULL                    | Customer city         |
| state       | VARCHAR(50)  | NOT NULL                    | Customer state        |
| pincode     | VARCHAR(10)  | NOT NULL                    | Postal code           |
| created_at  | TIMESTAMP    | DEFAULT CURRENT_TIMESTAMP   | Account creation date |

## 🔐 Database Constraints

The project uses different constraints to maintain data integrity:

### Primary Key

Uniquely identifies each customer record.

### Auto Increment

Automatically generates a unique customer ID.

### NOT NULL

Prevents required fields from being empty.

### UNIQUE

Prevents duplicate email addresses and phone numbers.

### DEFAULT

Automatically stores the current date and time for account creation.

## 🛠️ Technologies

* **Database:** MySQL
* **Query Language:** SQL
* **Database Design:** Relational Database Model

## 📁 Project Structure

```text
E-Commerce-Database-Management-System/
│
├── README.md
├── requirement_analysis.sql
├── customer_table.sql
├── product_table.sql
├── order_table.sql
├── payment_table.sql
├── seller_table.sql
└── review_table.sql
```

## 🚀 Future Enhancements

The project can be extended by adding:

* Product inventory management
* Order tracking
* Shipment management
* Payment status tracking
* Customer login and authentication
* Advanced reporting
* Sales analytics
* Admin dashboard



## 📄 Conclusion

The E-Commerce Database Management System provides a structured approach for storing and managing e-commerce business data. By using relational database concepts and constraints, the system helps maintain data consistency, accuracy, and integrity.
