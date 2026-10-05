# ServiceHub-Service-Management-Database

# SQL Database Project

## 📌 Project Overview

This project is a **SQL-based database project** designed to store, organize, and retrieve structured data efficiently.

The project demonstrates how a relational database can be created and managed using SQL. It includes database and table creation, inserting records, retrieving information, filtering data, sorting results, and performing different types of SQL operations.

The main purpose of this project is to practice **SQL and relational database concepts** using a practical dataset.

---

## 🎯 Objectives

The main objectives of this project are:

* To understand the fundamentals of SQL.
* To create and manage a relational database.
* To create tables with appropriate columns and data types.
* To insert and manage records.
* To retrieve useful information using SQL queries.
* To use filtering and sorting techniques.
* To perform calculations using aggregate functions.
* To understand relationships between tables.
* To practice SQL joins and subqueries.
* To develop practical database-management skills.

---

## 🗄️ Database Structure

The project follows a relational database structure.

### Main Database Components

The database contains tables that store related information. Each table consists of:

* **Primary Key** – Uniquely identifies each record.
* **Columns** – Store specific attributes of the data.
* **Rows/Records** – Store individual entries.
* **Foreign Key** – Connects related tables when required.

### Example Structure

```text
Database
│
├── Table 1
│   ├── ID (Primary Key)
│   ├── Name
│   ├── Category
│   └── Other Details
│
├── Table 2
│   ├── ID (Primary Key)
│   ├── Related_ID (Foreign Key)
│   └── Other Details
│
└── Table 3
    ├── ID (Primary Key)
    └── Other Details
```

> Replace the example table and column names above with the exact tables used in your project.

---

## 🛠️ SQL Concepts Used

The project demonstrates several important SQL concepts.

### 1. Database Creation

```sql
CREATE DATABASE database_name;
```

Creates a new database.

### 2. Table Creation

```sql
CREATE TABLE table_name (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    category VARCHAR(50)
);
```

Creates a table with columns and data types.

### 3. Inserting Data

```sql
INSERT INTO table_name
VALUES (1, 'Example', 'Category');
```

Adds records to a table.

### 4. Selecting Data

```sql
SELECT * FROM table_name;
```

Retrieves all records from a table.

### 5. Filtering Data

```sql
SELECT *
FROM table_name
WHERE category = 'Example';
```

Retrieves records that satisfy a condition.

### 6. Sorting Data

```sql
SELECT *
FROM table_name
ORDER BY name ASC;
```

Sorts the result.

### 7. Aggregate Functions

The project can use functions such as:

* `COUNT()`
* `SUM()`
* `AVG()`
* `MIN()`
* `MAX()`

Example:

```sql
SELECT COUNT(*) 
FROM table_name;
```

### 8. GROUP BY

```sql
SELECT category, COUNT(*)
FROM table_name
GROUP BY category;
```

Groups records based on a column.

### 9. HAVING

```sql
SELECT category, COUNT(*)
FROM table_name
GROUP BY category
HAVING COUNT(*) > 1;
```

Filters grouped results.

### 10. JOIN

Joins allow information from multiple related tables to be combined.

```sql
SELECT a.name, b.category
FROM table_a a
JOIN table_b b
ON a.id = b.id;
```

### 11. Subqueries

A query can be placed inside another query to retrieve more specific information.

```sql
SELECT *
FROM table_name
WHERE id IN (
    SELECT id
    FROM another_table
);
```

### 12. UPDATE

```sql
UPDATE table_name
SET category = 'New Category'
WHERE id = 1;
```

Updates existing records.

### 13. DELETE

```sql
DELETE FROM table_name
WHERE id = 1;
```

Deletes records that meet a condition.

---

## 💻 Technologies Used

* **SQL**
* Relational Database Management System (RDBMS)
* MySQL / SQL-compatible database system
* SQL queries for data manipulation and analysis

---

## ▶️ How to Run

### Step 1: Install a Database System

Install an SQL database system such as **MySQL** and optionally a GUI such as MySQL Workbench.

### Step 2: Create the Database

Open your SQL environment and run:

```sql
CREATE DATABASE database_name;
```

### Step 3: Select the Database

```sql
USE database_name;
```

### Step 4: Create the Tables

Run the `CREATE TABLE` statements from the project SQL file.

### Step 5: Insert the Data

Run the `INSERT INTO` statements to add the project data.

### Step 6: Run SQL Queries

Execute the SELECT, JOIN, GROUP BY, aggregate, subquery, UPDATE, and other queries included in the project.

### Step 7: View the Results

The SQL client will display the results of each query.

---

## 📂 Suggested Project Structure

```text
SQL-Project/
│
├── README.md
├── database.sql
└── screenshots/
    ├── database.png
    └── query-results.png
```

---

## 📊 Expected Outcome

After completing the project, users should be able to:

* Create a relational database.
* Create and manage tables.
* Insert and modify records.
* Retrieve useful information using SQL.
* Filter and sort data.
* Perform calculations using aggregate functions.
* Combine information from multiple tables.
* Use SQL queries for basic data analysis.

---

## 👨‍💻 Author

**Muhammed Abnas**

Data Science Student

---

## 📜 License

This project is created for **educational and learning purposes**.
