# SQL Fundamentals & Relational Databases 🗄️

## 1. What is a Database?
A **Database** is any collection of related information. It can be something as simple as a grocery list or as complex as a global social media user base.

### Examples:
* 📖 Phone Books
* 🛒 Shopping Lists
* ✅ To-Do Lists
* 👥 Facebook User Bases

### Storage Methods
Databases aren't limited to computers; they can be stored in various ways:
* On physical paper
* In your mind
* On a computer
* Within a Jupyter Notebook

---

## 2. Core SQL Concepts

### Database Management System (DBMS)
A DBMS is the software used to create, maintain, and secure databases. It serves as the interface between the data and the user.



### Relational vs. Non-Relational (NoSQL)
* **Relational Databases (RDBMS):** Data is organized into tables with predefined relationships. They use **SQL** (Structured Query Language).
* **Non-Relational Databases (NoSQL):** Data is stored in formats like documents, graphs, or key-value pairs (e.g., MongoDB).

---

## 3. SQL Data Types
When creating tables, you must define the type of data each column will hold:

| Data Type | Description | Example |
| :--- | :--- | :--- |
| `INT` | Whole numbers | `101` |
| `DECIMAL(M,N)` | Exact decimal numbers | `DECIMAL(10,2)` |
| `VARCHAR(L)` | Variable-length strings | `VARCHAR(50)` |
| `DATE` | Calendar dates | `YYYY-MM-DD` |
| `TIMESTAMP` | Date and time combined | `2023-10-27 10:00:00` |

---

## 4. Data Definition & Manipulation (CRUD)

### Creating a Table
Use the `CREATE TABLE` command to define the schema of your data:

```sql
CREATE TABLE employee (
    emp_id INT PRIMARY KEY,
    first_name VARCHAR(40),
    last_name VARCHAR(40),
    birth_day DATE,
    sex VARCHAR(1),
    salary INT,
    super_id INT,
    branch_id INT
);
