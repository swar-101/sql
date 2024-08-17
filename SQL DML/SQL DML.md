# SQL Data Manipulation Language (DML)
## Introduction
Data Manipulation Language (DML) is a subset of SQL commands used to manage and manipulate data stored in relational databases. The key DML operations are **CRUD**: Create, Read, Update, and Delete.

## Table of Contents
1. [INSERT](#insert)
2. [SELECT](#select)
3. [UPDATE](#update)
4. [DELETE](#delete)
5. [Summary](#summary)

---

## INSERT

### Description
The `INSERT` statement is used to add new rows (records) into a table.

### Syntax
```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

### Example
```sql
INSERT INTO employees (first_name, last_name, department, salary)
VALUES ('John', 'Doe', 'Engineering', 75000);
```

### Explanation
- **table_name**: The table where the new row will be added.
- **(column1, column2, ...)**: The columns that will receive the specified values.
- **VALUES (value1, value2, ...)**: The values to be inserted into the specified columns.

---

## SELECT

### Description
The `SELECT` statement is used to retrieve data from one or more tables.

### Syntax
```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

### Example
```sql
SELECT first_name, last_name, salary
FROM employees
WHERE department = 'Engineering';
```

### Explanation
- **SELECT column1, column2, ...**: Specifies the columns to retrieve.
- **FROM table_name**: Indicates the table to query.
- **WHERE condition**: Filters the result set to include only rows that meet the specified condition.

---

## UPDATE

### Description
The `UPDATE` statement is used to modify existing records in a table.

### Syntax
```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

### Example
```sql
UPDATE employees
SET salary = 80000
WHERE first_name = 'John' AND last_name = 'Doe';
```

### Explanation
- **SET column1 = value1, ...**: Specifies the columns and new values.
- **WHERE condition**: Ensures that only rows matching the condition are updated.

---

## DELETE

### Description
The `DELETE` statement is used to remove existing records from a table.

### Syntax
```sql
DELETE FROM table_name
WHERE condition;
```

### Example
```sql
DELETE FROM employees
WHERE last_name = 'Doe';
```

### Explanation
- **DELETE FROM table_name**: Specifies the table from which to delete rows.
- **WHERE condition**: Filters the rows to be deleted. If omitted, **all rows** in the table will be deleted.

---

## Summary

The SQL Data Manipulation Language (DML) allows you to perform essential operations on your database data: inserting, retrieving, updating, and deleting records. Mastering these commands will enable you to effectively manage and manipulate the data in your SQL databases.
