# MySQL Query Interview Questions and Answers

This repository contains **500 MySQL query-related interview questions and answers**. It is divided into multiple categories, covering everything from basic SQL queries to advanced MySQL architecture, performance tuning, replication, and clustering.

---

## 📘 Table of Contents

1.  [Basic SQL Queries (1–50)](#1-basic-sql-queries-150)
2.  [Joins (51-100)](#2-joins-51-100) <!-- Note: Adjust range if needed based on actual content -->
3.  [Aggregate Functions and Grouping (151–200)](#3-aggregate-functions-and-grouping-151200) <!-- Note: This seems out of order based on the provided text. Reordering/renumbering might be needed -->
4.  [Subqueries and Set Operations (101–150)](#4-subqueries-and-set-operations-101150) <!-- Note: This seems out of order based on the provided text. Reordering/renumbering might be needed -->
5.  [Indexes and Keys (201–250)](#5-indexes-and-keys-201250)
6.  [Data Types and Constraints (51–60)](#6-data-types-and-constraints-5160) <!-- Note: Ranges overlap/are out of sequence -->
7.  [Operators (Specific Range Missing)](#7-operators-specific-range-missing)
8.  [Data Definition Language (DDL) (Specific Range Missing)](#8-data-definition-language-ddl-specific-range-missing)
9.  [Data Manipulation Language (DML) (Specific Range Missing)](#9-data-manipulation-language-dml-specific-range-missing)
10. [Views and Temporary Tables (Specific Range Missing)](#10-views-and-temporary-tables-specific-range-missing)
11. [MySQL Functions (101–110)](#11-mysql-functions-101110) <!-- Note: Ranges overlap/are out of sequence -->
12. [Stored Procedures (Specific Range Missing)](#12-stored-procedures-specific-range-missing)
13. [Transactions (Specific Range Missing)](#13-transactions-specific-range-missing)
14. [Triggers (Specific Range Missing)](#14-triggers-specific-range-missing)
15. [JSON Data Type (Specific Range Missing)](#15-json-data-type-specific-range-missing)
16. [User Management (Specific Range Missing)](#16-user-management-specific-range-missing)
17. [Indexes (Specific Range Missing)](#17-indexes-specific-range-missing) <!-- Note: Duplicate category name -->
18. [Performance Optimization (Specific Range Missing)](#18-performance-optimization-specific-range-missing)
19. [Joins (Specific Range Missing)](#19-joins-specific-range-missing) <!-- Note: Duplicate category name -->
20. [Replication (Specific Range Missing)](#20-replication-specific-range-missing)
21. [Backup and Miscellaneous (Specific Range Missing)](#21-backup-and-miscellaneous-specific-range-missing)
22. [Views (Specific Range Missing)](#22-views-specific-range-missing) <!-- Note: Duplicate category name -->
23. [Temporary Tables (Specific Range Missing)](#23-temporary-tables-specific-range-missing) <!-- Note: Duplicate category name -->
24. [Common Functions (Specific Range Missing)](#24-common-functions-specific-range-missing)
25. [Security (Specific Range Missing)](#25-security-specific-range-missing)
26. [Configuration and Administration (Specific Range Missing)](#26-configuration-and-administration-specific-range-missing)
27. [Triggers (Specific Range Missing)](#27-triggers-specific-range-missing) <!-- Note: Duplicate category name -->
28. [Stored Procedures & Functions (431–440)](#28-stored-procedures--functions-431440)
29. [Transactions (Specific Range Missing)](#29-transactions-specific-range-missing) <!-- Note: Duplicate category name -->
30. [Partitioning (441–450)](#30-partitioning-441450)
31. [JSON (Specific Range Missing)](#31-json-specific-range-missing) <!-- Note: Duplicate category name -->
32. [Performance Tuning (471–480)](#32-performance-tuning-471480)
33. [Logging (Specific Range Missing)](#33-logging-specific-range-missing)
34. [Replication (451–460)](#34-replication-451460) <!-- Note: Duplicate category name -->
35. [Events (Specific Range Missing)](#35-events-specific-range-missing)
36. [Troubleshooting (Specific Range Missing)](#36-troubleshooting-specific-range-missing)
37. [User Management (Specific Range Missing)](#37-user-management-specific-range-missing) <!-- Note: Duplicate category name -->
38. [Advanced Indexing & Query Optimization (Specific Range Missing)](#38-advanced-indexing--query-optimization-specific-range-missing)
39. [Backup and Recovery (Specific Range Missing)](#39-backup-and-recovery-specific-range-missing)
40. [Migration & Compatibility (Specific Range Missing)](#40-migration--compatibility-specific-range-missing)
41. [Miscellaneous (391–400)](#41-miscellaneous-391400)
42. [Transactions & Isolation (401–410)](#42-transactions--isolation-401410) <!-- Note: Duplicate category name -->
43. [JSON in MySQL (411–420)](#43-json-in-mysql-411420) <!-- Note: Duplicate category name -->
44. [Views (421–430)](#44-views-421430) <!-- Note: Duplicate category name -->
45. [Stored Routines & Functions (431–440)](#45-stored-routines--functions-431440) <!-- Note: Duplicate category name -->
46. [Partitioning (441–450)](#46-partitioning-441450) <!-- Note: Duplicate category name -->
47. [Replication & High Availability (451–460)](#47-replication--high-availability-451460) <!-- Note: Duplicate category name -->
48. [MySQL Cluster & Scaling (461–470)](#48-mysql-cluster--scaling-461470)
49. [Performance Tuning (471–480)](#49-performance-tuning-471480) <!-- Note: Duplicate category name -->
50. [Monitoring & Maintenance (481–490)](#50-monitoring--maintenance-481490)
51. [Advanced & Scenario-Based (491–500)](#51-advanced--scenario-based-491500)

*(Note: The Table of Contents was auto-generated based on the provided text. Some categories appear duplicated or out of sequence, and many lack specific question ranges in the original text. You may need to manually review and adjust the numbering, ranges, category names, and links for accuracy and logical flow.)*

---

 ### 1. Basic SQL Queries (1–50)

**Q: What is the syntax to select all columns from a table?**
A: `SELECT * FROM table_name;`

**Q: How do you retrieve only unique values from a column?**
A: `SELECT DISTINCT column_name FROM table_name;`

**Q: How do you rename a column in the result set?**
A: `SELECT column_name AS alias_name FROM table_name;`

**Q: How do you filter records using the WHERE clause?**
A: `SELECT * FROM table_name WHERE condition;`

**Q: What does the LIMIT clause do?**
A: It restricts the number of rows returned: `SELECT * FROM table LIMIT 10;`

**Q: How do you sort results in ascending or descending order?**
A: `SELECT * FROM table ORDER BY column ASC|DESC;`

**Q: How do you fetch records where a column value is NULL?**
A: `SELECT * FROM table WHERE column IS NULL;`

**Q: How to check if a value exists in a list?**
A: `SELECT * FROM table WHERE column IN ('A', 'B');`

**Q: How do you perform a case-insensitive search?**
A: `SELECT * FROM table WHERE LOWER(column) = 'value';`

**Q: How to get the current date?**
A: `SELECT CURDATE();`

*(Questions 11-50 seem to be missing from this section in the provided text)*

---

## 2. Joins (51-100)

**Q: What is an INNER JOIN?**
A: Returns rows with matching values in both tables.

**Q: Write an INNER JOIN query between employees and departments.**
A:
```sql
SELECT e.name, d.name
FROM employees e
INNER JOIN departments d ON e.dept_id = d.id;
```

**Q: What is a LEFT JOIN?**
A: Returns all rows from the left table, matched with right table rows (NULL if no match).

**Q: Difference between LEFT JOIN and RIGHT JOIN?**
A: LEFT JOIN gets all rows from the left; RIGHT JOIN gets all from the right.

**Q: What is a CROSS JOIN?**
A: Cartesian product of two tables.

**Q: How do you join more than two tables?**
A: By chaining JOIN clauses:
```sql
SELECT *
FROM A
JOIN B ON A.id = B.a_id
JOIN C ON B.id = C.b_id;
```

**Q: Can you use WHERE with JOINs?**
A: Yes, to further filter the joined results.

**Q: How to find employees without departments?**
A: Use LEFT JOIN and check for NULL in department table.

**Q: What is a SELF JOIN?**
A: Joining a table with itself.

**Q: What is a NATURAL JOIN?**
A: A JOIN that automatically uses all matching column names.

*(Questions 61-100 seem to be missing from this section in the provided text)*

---

## 3. Aggregate Functions and Grouping (151–200)

**Q: How to get the total count of records?**
A: `SELECT COUNT(*) FROM table;`

**Q: How to calculate average salary?**
A: `SELECT AVG(salary) FROM employees;`

**Q: What is GROUP BY used for?**
A: To group rows sharing a property and aggregate them.

**Q: Write a query to find total sales by region.**
A:
```sql
SELECT region, SUM(sales)
FROM orders
GROUP BY region;
```

**Q: How do you filter grouped records?**
A: Use HAVING clause.

**Q: What is the difference between WHERE and HAVING?**
A: WHERE filters rows; HAVING filters aggregated results.

**Q: Write a query to count employees in each department.**
A:
```sql
SELECT dept_id, COUNT(*)
FROM employees
GROUP BY dept_id;
```

**Q: How to find the maximum and minimum salary?**
A: `SELECT MAX(salary), MIN(salary) FROM employees;`

**Q: Can you use aggregate functions in WHERE clause?**
A: No, use them in HAVING clause.

**Q: What is the result of SUM(NULL)?**
A: NULL.

*(Questions 161-200 seem to be missing from this section in the provided text)*

---

## 4. Subqueries and Set Operations (101–150)

**Q: What is a subquery?**
A: A query nested inside another query.

**Q: Can a subquery return multiple rows?**
A: Yes, if used with IN, EXISTS, etc.

**Q: How to get employees with salary greater than average salary?**
A:
```sql
SELECT *
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```

**Q: What is a correlated subquery?**
A: A subquery that depends on the outer query.

**Q: Difference between IN and EXISTS?**
A: IN checks values; EXISTS checks for row existence.

**Q: Can subqueries be used in SELECT clause?**
A: Yes.

**Q: Write a query using subquery in FROM clause.**
A:
```sql
SELECT avg_salary
FROM (SELECT AVG(salary) AS avg_salary FROM employees) AS temp;
```

**Q: Can we use subquery in UPDATE statement?**
A: Yes.

**Q: What is the use of ANY and ALL with subqueries?**
A: To compare value with any/all values from subquery result.

**Q: Can subqueries return NULL?**
A: Yes.

*(Questions 111-150 seem to be missing from this section in the provided text)*

---

## 5. Indexes and Keys (201–250)

**Q: What is an index in MySQL?**
A: A data structure to speed up queries.

**Q: How to create an index?**
A: `CREATE INDEX idx_name ON table(column);`

**Q: What is a primary key?**
A: A unique identifier for records.

**Q: What is a unique key?**
A: Ensures all values in a column are unique.

**Q: Difference between primary and unique key?**
A: Primary key = unique + not null.

**Q: How to check existing indexes?**
A: `SHOW INDEXES FROM table_name;`

**Q: How to remove an index?**
A: `DROP INDEX index_name ON table_name;`

**Q: What is EXPLAIN used for?**
A: To analyze and optimize query performance.

**Q: What is the slow query log?**
A: A MySQL feature to log long-running queries.

**Q: How to optimize a slow SELECT query?**
A: Use proper indexes, avoid *, limit result set, and analyze using EXPLAIN.

*(Questions 211-250 seem to be missing from this section in the provided text)*

---

## 6. Data Types and Constraints (51–60)

*(Note: This section seems out of order and overlaps with others. Review required.)*

**Q: What are the common data types in MySQL?**
A: INT, VARCHAR, TEXT, DATE, DATETIME, FLOAT, DOUBLE, BOOLEAN.

**Q: Difference between CHAR and VARCHAR?**
A: CHAR is fixed-length, VARCHAR is variable-length.

**Q: What is the maximum length of a VARCHAR?**
A: Up to 65,535 bytes (depends on row format and character set).

**Q: What is the use of NOT NULL constraint?**
A: Prevents null values in a column.

**Q: What is the DEFAULT constraint?**
A: Sets a default value if none is provided during insertion.

**Q: How do you define a column as UNIQUE?**
A: `UNIQUE (column_name)` during table creation.

**Q: Can a table have multiple UNIQUE keys?**
A: Yes.

**Q: What is the difference between NOW() and CURDATE()?**
A: `NOW()` gives current date & time; `CURDATE()` gives only the date.

**Q: What are ENUM and SET types?**
A: ENUM stores a single value from a list, SET stores multiple values.

**Q: Can you use AUTO_INCREMENT on multiple columns?**
A: No, only one column per table.

---

## 7. Operators (Specific Range Missing)

**Q: What does the BETWEEN operator do?**
A: Filters data within a range: `BETWEEN 10 AND 20`.

**Q: What is the LIKE operator used for?**
A: Pattern matching in strings.

**Q: What does % mean in a LIKE clause?**
A: Wildcard for zero or more characters.

**Q: How to use NOT LIKE?**
A: `SELECT * FROM table WHERE column NOT LIKE 'A%';`

**Q: How to search for values ending with "son"?**
A: `WHERE name LIKE '%son'`

**Q: How to combine filters with AND/OR?**
A: `WHERE column1 = 'A' AND column2 = 'B'`

**Q: How to exclude nulls in a query?**
A: `WHERE column IS NOT NULL`

**Q: How to get records with either condition A or B true?**
A: `WHERE conditionA OR conditionB`

**Q: How to get data where column is not in a list?**
A: `WHERE column NOT IN (val1, val2)`

**Q: Can WHERE be used with aggregate functions?**
A: No, use HAVING instead.

---

## 8. Data Definition Language (DDL) (Specific Range Missing)

**Q: How do you create a table?**
A:
```sql
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100)
);
```

**Q: How do you modify a column's data type?**
A: `ALTER TABLE table_name MODIFY column_name NEWTYPE;`

**Q: How to add a new column to an existing table?**
A: `ALTER TABLE table_name ADD column_name DATATYPE;`

**Q: How to rename a table?**
A: `RENAME TABLE old_name TO new_name;`

**Q: How to delete a column?**
A: `ALTER TABLE table_name DROP COLUMN column_name;`

**Q: How to drop a table?**
A: `DROP TABLE table_name;`

**Q: What is the difference between DROP and DELETE?**
A: DROP removes the table structure; DELETE removes data only.

**Q: What does TRUNCATE do?**
A: Removes all data and resets AUTO_INCREMENT.

**Q: How to rename a column?**
A: `ALTER TABLE table_name CHANGE old_column new_column DATATYPE;`

**Q: What happens if you DROP a table with foreign keys?**
A: It fails unless you remove constraints or use `SET foreign_key_checks = 0;`

---

## 9. Data Manipulation Language (DML) (Specific Range Missing)

**Q: How to insert data into a table?**
A: `INSERT INTO table (col1, col2) VALUES (val1, val2);`

**Q: How to update existing records?**
A: `UPDATE table SET column = value WHERE condition;`

**Q: How to delete records?**
A: `DELETE FROM table WHERE condition;`

**Q: What happens if you omit the WHERE clause in UPDATE?**
A: All rows are updated.

**Q: What happens if you omit the WHERE clause in DELETE?**
A: All rows are deleted.

**Q: How do you insert data from another table?**
A:
```sql
INSERT INTO table1 (col1, col2)
SELECT col1, col2 FROM table2;
```

**Q: Can you update multiple columns in one query?**
A: Yes: `SET col1 = val1, col2 = val2`

**Q: How do you insert multiple rows?**
A:
```sql
INSERT INTO table (col1, col2) VALUES (val1a, val2a), (val1b, val2b);
```

**Q: How do you prevent inserting duplicate records?**
A: Use `INSERT IGNORE` or `INSERT ... ON DUPLICATE KEY UPDATE`

**Q: What does REPLACE INTO do?**
A: Deletes existing row with same key and inserts a new one.

---

## 10. Views and Temporary Tables (Specific Range Missing)

**Q: What is a view in MySQL?**
A: A virtual table based on a SELECT query.

**Q: How to create a view?**
A:
```sql
CREATE VIEW view_name AS
SELECT col1, col2 FROM table;
```

**Q: Can you update data through a view?**
A: Yes, if the view is based on a single table without aggregation.

**Q: How to delete a view?**
A: `DROP VIEW view_name;`

**Q: What are temporary tables?**
A: Tables that exist only during a session.

**Q: How to create a temporary table?**
A: `CREATE TEMPORARY TABLE temp_table (...)`

**Q: Can you join a view and a table?**
A: Yes.

**Q: What happens to a TEMP table if the session closes?**
A: It is automatically deleted.

**Q: Can you index a view?**
A: Not directly; use materialized views for performance (not natively supported in MySQL).

**Q: What's the advantage of using views?**
A: Simplifies complex queries, improves security, and supports reusability.

---

## 11. MySQL Functions (101–110)

*(Note: This section seems out of order and overlaps with others. Review required.)*

**Q: What is a MySQL function?**
A: A built-in operation that performs a task and returns a value.

**Q: How to concatenate two strings in MySQL?**
A: `SELECT CONCAT('Hello', ' World');`

**Q: What does LENGTH() return?**
A: Number of bytes in a string.

**Q: How to extract a substring?**
A: `SELECT SUBSTRING('abcdef', 2, 3);` → returns bcd

**Q: How to convert text to uppercase?**
A: `SELECT UPPER('mysql');`

**Q: How to get current time in MySQL?**
A: `SELECT NOW();`

**Q: What does DATEDIFF() do?**
A: Returns the difference between two dates in days.

**Q: How to round a number in MySQL?**
A: `SELECT ROUND(123.456, 2);`

**Q: How to generate a random number?**
A: `SELECT RAND();`

**Q: What does COALESCE() do?**
A: Returns the first non-null value from a list.

---

## 12. Stored Procedures (Specific Range Missing)

**Q: What is a stored procedure?**
A: A saved set of SQL statements you can reuse.

**Q: How to create a stored procedure?**
A:
```sql
DELIMITER //
CREATE PROCEDURE proc_name()
BEGIN
  SELECT 'Hello';
END;
//
DELIMITER ;
```

**Q: How to call a stored procedure?**
A: `CALL proc_name();`

**Q: How to pass parameters to a procedure?**
A:
```sql
CREATE PROCEDURE proc(IN name VARCHAR(20))
BEGIN
  SELECT name;
END;
```

**Q: What are IN, OUT, and INOUT parameters?**
A: Input-only, output-only, and both.

**Q: How to drop a procedure?**
A: `DROP PROCEDURE proc_name;`

**Q: Can procedures return values?**
A: No, they return result sets, but can use OUT parameters.

**Q: Difference between procedure and function?**
A: Functions return values; procedures do not.

**Q: Can a procedure call another procedure?**
A: Yes, it's called nesting.

**Q: Are procedures transactional?**
A: Only if they contain transactional SQL and use InnoDB.

---

## 13. Transactions (Specific Range Missing)

**Q: What is a transaction?**
A: A group of SQL statements treated as a single unit.

**Q: What are the four properties of transactions?**
A: ACID – Atomicity, Consistency, Isolation, Durability.

**Q: How do you start a transaction?**
A: `START TRANSACTION;`

**Q: How do you save a transaction?**
A: `COMMIT;`

**Q: How do you undo a transaction?**
A: `ROLLBACK;`

**Q: What is a savepoint?**
A: A point to which you can roll back.

**Q: How to set a savepoint?**
A: `SAVEPOINT savepoint_name;`

**Q: How to roll back to a savepoint?**
A: `ROLLBACK TO savepoint_name;`

**Q: Which storage engine supports transactions?**
A: InnoDB.

**Q: Can you nest transactions in MySQL?**
A: Not directly, but you can use savepoints to simulate nesting.

---

## 14. Triggers (Specific Range Missing)

**Q: What is a trigger in MySQL?**
A: A procedure that runs automatically when an event occurs on a table.

**Q: Which operations can fire a trigger?**
A: INSERT, UPDATE, DELETE.

**Q: How to create a trigger?**
A:
```sql
CREATE TRIGGER before_insert
BEFORE INSERT ON table_name
FOR EACH ROW
BEGIN
  -- action
END;
```

**Q: What is the difference between BEFORE and AFTER triggers?**
A: BEFORE triggers run before the change, AFTER run after.

**Q: Can a table have multiple triggers for the same event?**
A: Yes, but with different timing (BEFORE/AFTER).

**Q: How to drop a trigger?**
A: `DROP TRIGGER trigger_name;`

**Q: Can triggers call stored procedures?**
A: Yes.

**Q: What is the NEW keyword in triggers?**
A: Refers to the new row in INSERT/UPDATE.

**Q: What is the OLD keyword in triggers?**
A: Refers to the row being deleted or updated.

**Q: Can you update the same table inside its own trigger?**
A: It's not recommended — can cause recursion or errors.

---

## 15. JSON Data Type (Specific Range Missing)

**Q: Does MySQL support JSON data type?**
A: Yes, from MySQL 5.7 onwards.

**Q: How to insert JSON data?**
A: `INSERT INTO table (data) VALUES ('{"key":"value"}');`

**Q: How to extract a value from JSON?**
A: `SELECT JSON_EXTRACT(data, '$.key') FROM table;`

**Q: What does JSON_OBJECT() do?**
A: Creates a JSON object.

**Q: How to search inside a JSON field?**
A: Use `JSON_CONTAINS()` or `JSON_EXTRACT()` in WHERE.

---

## 16. User Management (Specific Range Missing)

**Q: How to create a new MySQL user?**
A: `CREATE USER 'user'@'localhost' IDENTIFIED BY 'pass';`

**Q: How to grant privileges to a user?**
A: `GRANT ALL PRIVILEGES ON db.* TO 'user'@'localhost';`

**Q: How to see current user's privileges?**
A: `SHOW GRANTS FOR CURRENT_USER;`

**Q: How to remove a user?**
A: `DROP USER 'user'@'localhost';`

**Q: How to apply changes after GRANT?**
A: `FLUSH PRIVILEGES;`

---

## 17. Indexes (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is an index in MySQL?**
A: A data structure that improves the speed of data retrieval.

**Q: How do you create an index?**
A: `CREATE INDEX idx_name ON table_name (column);`

**Q: Types of indexes in MySQL?**
A: PRIMARY, UNIQUE, INDEX (non-unique), FULLTEXT, SPATIAL.

**Q: Can you index multiple columns?**
A: Yes, it's called a composite index.

**Q: How do indexes affect INSERTs?**
A: They slow down INSERT/UPDATE because indexes must be updated.

**Q: How to see all indexes of a table?**
A: `SHOW INDEXES FROM table_name;`

**Q: What is a covering index?**
A: An index that contains all the columns required by the query.

**Q: What is the difference between clustered and non-clustered index?**
A: InnoDB has clustered index (based on PRIMARY key), MyISAM doesn't support it.

**Q: How to drop an index?**
A: `DROP INDEX idx_name ON table_name;`

**Q: When should you not use indexes?**
A: On columns with high update frequency or low selectivity (e.g., boolean columns).

---

## 18. Performance Optimization (Specific Range Missing)

**Q: What is EXPLAIN used for?**
A: To analyze and optimize a SELECT query.

**Q: What does EXPLAIN SELECT * FROM table; show?**
A: Query execution plan – table access, index usage, row estimate.

**Q: What is the slow query log?**
A: A log of queries that take longer than a threshold.

**Q: How to enable slow query log?**
A: `SET GLOBAL slow_query_log = 1;`

**Q: What is a subquery?**
A: A query nested within another query.

**Q: What is a correlated subquery?**
A: A subquery that depends on the outer query.

**Q: How to limit result rows?**
A: Use LIMIT, e.g., `SELECT * FROM table LIMIT 10;`

**Q: What is query caching?**
A: Storing results of queries to serve repeated requests faster (deprecated in latest versions).

**Q: How can JOINs impact performance?**
A: Poor indexing or large table scans can slow them down.

**Q: What is the benefit of using SELECT column over SELECT *?**
A: Reduces I/O and improves performance.

---

## 19. Joins (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is an inner join?**
A: Returns matching rows from both tables.

**Q: What is a left join?**
A: Returns all rows from the left table, matching rows from the right.

**Q: What is a right join?**
A: Returns all rows from the right table, matching rows from the left.

**Q: What is a full outer join in MySQL?**
A: MySQL doesn't support it directly — simulate with UNION.

**Q: How to simulate full outer join?**
A:
```sql
SELECT * FROM A LEFT JOIN B ON ...
UNION
SELECT * FROM A RIGHT JOIN B ON ...;
```

**Q: What is a cross join?**
A: Produces the Cartesian product of two tables.

**Q: What is a self join?**
A: A table joined with itself using aliases.

**Q: Can you join more than two tables?**
A: Yes, multiple joins are allowed.

**Q: What's the use of ON vs USING in JOINs?**
A: ON allows different column names, USING assumes same column names.

**Q: Which join is faster: INNER or OUTER?**
A: INNER JOIN is usually faster due to fewer data comparisons.

---

## 20. Replication (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is replication in MySQL?**
A: Copying data from one server (master) to another (slave).

**Q: Types of replication?**
A: Master-Slave, Master-Master, Group Replication.

**Q: What is binary log?**
A: A log of all changes to the database; used for replication.

**Q: How do you start replication?**
A: Configure master/slave and start replication threads.

**Q: How to check replication status?**
A: `SHOW SLAVE STATUS\G`

**Q: What is GTID in replication?**
A: Global Transaction Identifier – uniquely identifies each transaction.

**Q: What is the role of relay log?**
A: Stores changes from master on the slave.

**Q: How to stop replication safely?**
A: `STOP SLAVE;` or `STOP REPLICA;`

**Q: What is mysqldump?**
A: A tool to export MySQL data and structure to a file.

**Q: How to backup only table structure?**
A: `mysqldump -d -u user -p db_name > structure.sql`

---

## 21. Backup and Miscellaneous (Specific Range Missing)

**Q: How to find duplicate records?**
A:
```sql
SELECT column, COUNT(*)
FROM table
GROUP BY column
HAVING COUNT(*) > 1;
```

**Q: How to delete duplicate records but keep one?**
A:
```sql
DELETE t1 FROM table t1
JOIN table t2
ON t1.id > t2.id AND t1.col = t2.col;
```

**Q: How to check MySQL version?**
A: `SELECT VERSION();`

**Q: How to kill a running query?**
A: `KILL process_id;`

**Q: What is the use of SHOW PROCESSLIST?**
A: Shows running threads and queries.

**Q: How to find long-running queries?**
A: Use `SHOW FULL PROCESSLIST` or slow query log.

**Q: How to reset AUTO_INCREMENT value?**
A: `ALTER TABLE table_name AUTO_INCREMENT = 1;`

**Q: How to check table size?**
A: Use `information_schema.TABLES` or `SHOW TABLE STATUS;`

**Q: What is the difference between logical and physical backup?**
A: Logical: SQL dump; Physical: raw data files.

**Q: How to restore a MySQL dump?**
A: `mysql -u root -p db_name < dump.sql`

---

## 22. Views (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is a view in MySQL?**
A: A virtual table based on the result of a SQL query.

**Q: How to create a view?**
A:
```sql
CREATE VIEW view_name AS
SELECT column1, column2 FROM table WHERE condition;
```

**Q: Can you update data through a view?**
A: Yes, if the view references a single table without GROUP BY or aggregate functions.

**Q: How to drop a view?**
A: `DROP VIEW view_name;`

**Q: How to list all views in a database?**
A: `SHOW FULL TABLES IN db_name WHERE TABLE_TYPE = 'VIEW';`

**Q: How to update a view?**
A: `CREATE OR REPLACE VIEW view_name AS SELECT ...;`

**Q: What is an updatable view?**
A: A view where INSERT, UPDATE, DELETE operations are allowed.

**Q: Can you join tables in a view?**
A: Yes, views can be based on complex joins.

**Q: What is the main use of views?**
A: Simplify complex queries, abstract data access, and enhance security.

**Q: Can you use ORDER BY in a view?**
A: Yes, but it's ignored unless used with LIMIT.

---

## 23. Temporary Tables (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is a temporary table?**
A: A table that exists only during the session.

**Q: How to create a temporary table?**
A: `CREATE TEMPORARY TABLE temp_table (...);`

**Q: When is a temporary table destroyed?**
A: At the end of the session or connection.

**Q: Can two users create temporary tables with the same name?**
A: Yes, because they're session-specific.

**Q: Can you create indexes on a temporary table?**
A: Yes.

**Q: Difference between TEMPORARY and regular tables?**
A: Temporary tables are deleted automatically; regular tables persist.

**Q: Are temporary tables stored in memory?**
A: Depends — MEMORY engine or disk if too large.

**Q: How to drop a temporary table manually?**
A: `DROP TEMPORARY TABLE table_name;`

**Q: Can you use a temporary table in a stored procedure?**
A: Yes.

**Q: What happens if you try to create a temporary table with the same name?**
A: It overwrites the existing temporary table in your session.

---

## 24. Common Functions (Specific Range Missing)

**Q: What does IFNULL() do?**
A: Replaces NULL with a default value.

**Q: What does NULLIF() do?**
A: Returns NULL if two expressions are equal.

**Q: Difference between COALESCE() and IFNULL()?**
A: COALESCE() can take multiple arguments; IFNULL() only two.

**Q: What does FORMAT() do?**
A: Formats numbers with commas and decimals.
Example: `FORMAT(12345.678, 2)` → 12,345.68

**Q: What does STR_TO_DATE() do?**
A: Converts a string to a date using a format mask.

**Q: What does DATE_FORMAT() do?**
A: Formats a date into a string.

**Q: What is LPAD() / RPAD()?**
A: Pads strings on the left/right.
`LPAD('5', 3, '0')` → '005'

**Q: How to convert a string to an integer?**
A: Use `CAST('123' AS UNSIGNED);`

**Q: How to get the day name from a date?**
A: `SELECT DAYNAME(NOW());`

**Q: How to count distinct values?**
A: `SELECT COUNT(DISTINCT column) FROM table;`

---

## 25. Security (Specific Range Missing)

**Q: How to restrict user access to a database?**
A: Use GRANT with limited privileges.

**Q: How to revoke user privileges?**
A: `REVOKE SELECT ON db.* FROM 'user'@'host';`

**Q: How to set a password for a MySQL user?**
A: `ALTER USER 'user'@'host' IDENTIFIED BY 'password';`

**Q: What is SQL injection?**
A: A hacking technique to inject malicious SQL through input.

**Q: How to prevent SQL injection in MySQL?**
A: Use prepared statements and parameterized queries.

**Q: How to check which users exist in MySQL?**
A: `SELECT user, host FROM mysql.user;`

**Q: Can a user have access to multiple databases?**
A: Yes, assign privileges to each.

**Q: What is the role of the mysql database?**
A: It stores users, privileges, and system settings.

**Q: What is WITH GRANT OPTION?**
A: Allows a user to grant their privileges to others.

**Q: How to enforce SSL for a user?**
A: Grant privileges with REQUIRE SSL.

---

## 26. Configuration and Administration (Specific Range Missing)

**Q: How to change the default port of MySQL?**
A: Modify the `my.cnf` or `my.ini` file (default is 3306).

**Q: What is information_schema?**
A: A read-only database with metadata about other databases.

**Q: How to stop and start MySQL service?**
A:
Linux: `systemctl start|stop mysql`
Windows: via Services or `net start mysql`

**Q: How to check the size of a database?**
A:
```sql
SELECT table_schema AS db,
SUM(data_length + index_length)/1024/1024 AS size_mb
FROM information_schema.tables
GROUP BY table_schema;
```

**Q: How to change a table engine?**
A: `ALTER TABLE table_name ENGINE = InnoDB;`

**Q: How to defragment a table?**
A: Use `OPTIMIZE TABLE table_name;`

**Q: How to enable binary logging?**
A: Set `log-bin` in `my.cnf` and restart MySQL.

**Q: What is the purpose of FLUSH PRIVILEGES?**
A: Reloads privilege tables after GRANT/REVOKE.

**Q: What is a deadlock?**
A: Two transactions wait on each other to release resources.

**Q: How to detect deadlocks?**
A: Use `SHOW ENGINE INNODB STATUS;` to find deadlock info.

---

## 27. Triggers (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is a trigger in MySQL?**
A: A set of instructions automatically executed in response to events on a table (INSERT, UPDATE, DELETE).

**Q: How to create a trigger?**
A:
```sql
CREATE TRIGGER trg_name BEFORE INSERT ON table_name
FOR EACH ROW
BEGIN
   -- logic here
END;
```

**Q: What are the types of triggers?**
A: BEFORE INSERT, AFTER INSERT, BEFORE UPDATE, AFTER UPDATE, BEFORE DELETE, AFTER DELETE.

**Q: Can you create multiple triggers of the same type on one table?**
A: No. Only one BEFORE and one AFTER trigger allowed per event per table.

**Q: Can triggers call stored procedures?**
A: Yes, but they can't commit or roll back transactions.

**Q: Can triggers modify other tables?**
A: Yes, but not the same table where the trigger is defined (to avoid recursion).

**Q: How to drop a trigger?**
A: `DROP TRIGGER trigger_name;`

**Q: Are triggers executed per statement or per row?**
A: Per row (FOR EACH ROW).

**Q: How to list all triggers in a database?**
A: `SHOW TRIGGERS FROM db_name;`

**Q: Where are triggers stored?**
A: In the `information_schema.TRIGGERS` table.

---

## 28. Stored Procedures & Functions (431–440)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is a stored procedure?**
A: A precompiled set of SQL statements stored in the database.

**Q: How to create a stored procedure?**
A:
```sql
DELIMITER //
CREATE PROCEDURE proc_name()
BEGIN
  -- SQL logic
END //
DELIMITER ;
```

**Q: What is the difference between a stored procedure and function?**
A: Functions return a value; procedures may or may not.

**Q: How to call a stored procedure?**
A: `CALL proc_name();`

**Q: How to return a value from a stored function?**
A: `RETURN some_value;`

**Q: How to drop a procedure or function?**
A: `DROP PROCEDURE proc_name;` or `DROP FUNCTION func_name;`

**Q: What are IN, OUT, INOUT parameters?**
A: IN: Passes value, OUT: Returns value, INOUT: Passes and returns

**Q: Can procedures use control-flow statements (IF, WHILE)?**
A: Yes.

**Q: Can a stored procedure return a result set?**
A: Yes, by using SELECT statements inside it.

**Q: Where are procedures/functions stored?**
A: In `mysql.proc` or `information_schema.ROUTINES`.

---

## 29. Transactions (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: What is a transaction in MySQL?**
A: A group of SQL statements treated as a single unit.

**Q: Which engines support transactions?**
A: InnoDB supports transactions; MyISAM does not.

**Q: What are the ACID properties?**
A: Atomicity, Consistency, Isolation, Durability.

**Q: How to start a transaction?**
A:
```sql
START TRANSACTION;
-- SQL statements
COMMIT;
```

**Q: What does COMMIT do?**
A: Saves the changes made in the transaction.

**Q: What does ROLLBACK do?**
A: Undoes the changes made during the transaction.

**Q: What is SAVEPOINT?**
A: A point within a transaction to which you can roll back.

**Q: What is the default isolation level in MySQL?**
A: REPEATABLE READ.

**Q: How to change isolation level?**
A: `SET SESSION TRANSACTION ISOLATION LEVEL READ COMMITTED;`

**Q: What is the difference between COMMIT and ROLLBACK?**
A: COMMIT saves changes; ROLLBACK discards them.

---

## 30. Partitioning (441–450)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is partitioning?**
A: Dividing a table into smaller, more manageable pieces.

**Q: Benefits of partitioning?**
A: Better performance and manageability for large tables.

**Q: Types of partitioning?**
A: RANGE, LIST, HASH, KEY.

**Q: Can you index partitioned tables?**
A: Yes, but there are restrictions on primary and unique keys.

**Q: How to partition a table by range?**
A:
```sql
PARTITION BY RANGE (year_column) (
  PARTITION p1 VALUES LESS THAN (2020),
  PARTITION p2 VALUES LESS THAN (2025)
);
```

**Q: Can you drop a partition?**
A: Yes: `ALTER TABLE table DROP PARTITION p_name;`

**Q: Can you add partitions to an existing table?**
A: Yes: `ALTER TABLE table ADD PARTITION (...)`

**Q: Can foreign keys be used in partitioned tables?**
A: No, MySQL does not allow foreign keys on partitioned tables.

**Q: How to check partition info?**
A: Use `information_schema.PARTITIONS`.

**Q: Are all engines supported for partitioning?**
A: No, only InnoDB and NDB support it.

---

## 31. JSON (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: Does MySQL support JSON data type?**
A: Yes, from MySQL 5.7 onward.

**Q: How to store JSON in MySQL?**
A: Use the JSON data type.

**Q: How to insert JSON data?**
A: `INSERT INTO table(json_col) VALUES ('{"name":"Rakesh", "age":30}');`

**Q: How to extract values from JSON?**
A: `SELECT JSON_EXTRACT(json_col, '$.name') FROM table;`

**Q: What is the difference between -> and ->> in MySQL JSON?**
A: `->` returns JSON type; `->>` returns text.

**Q: How to update a JSON key?**
A: Use `JSON_SET(json_col, '$.key', 'value')`

**Q: How to delete a key from JSON?**
A: Use `JSON_REMOVE(json_col, '$.key')`

**Q: How to check if a JSON key exists?**
A: `JSON_CONTAINS_PATH(json_col, 'one', '$.key')`

**Q: Can you index JSON fields?**
A: Yes, using generated columns and then indexing those.

**Q: How to pretty print JSON in MySQL?**
A: Use `JSON_PRETTY(json_col)`

---

## 32. Performance Tuning (471–480)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is the EXPLAIN keyword used for?**
A: It shows how MySQL executes a query and helps optimize performance.

**Q: How to find slow queries in MySQL?**
A: Enable `slow_query_log` and review the log file.

**Q: What is the Query Cache?**
A: It stores the result of SELECT queries for reuse. (Deprecated in MySQL 8.0)

**Q: How to see which queries are currently running?**
A: `SHOW FULL PROCESSLIST;`

**Q: How to identify unused indexes?**
A: Use `performance_schema` or tools like `pt-index-usage`.

**Q: What is the mysqltuner tool?**
A: A script to analyze MySQL performance and suggest improvements.

**Q: How to check table statistics?**
A: Use `SHOW TABLE STATUS;`

**Q: What is ANALYZE TABLE used for?**
A: Updates index statistics for better query planning.

**Q: When should you use FORCE INDEX?**
A: When the optimizer is choosing a poor index.

**Q: What is the difference between SHOW PROFILE and EXPLAIN?**
A: `SHOW PROFILE` shows resource usage; `EXPLAIN` shows query execution plan.

---

## 33. Logging (Specific Range Missing)

**Q: What are the types of logs in MySQL?**
A: Error log, General log, Slow query log, Binary log.

**Q: How to enable the slow query log?**
A: `SET GLOBAL slow_query_log = 1;`

**Q: What does the general log contain?**
A: All SQL queries sent to the server.

**Q: How to view the error log?**
A: Check the file specified in `my.cnf` under `log_error`.

**Q: What is the binary log used for?**
A: For replication and point-in-time recovery.

**Q: How to list binary logs?**
A: `SHOW BINARY LOGS;`

**Q: How to purge binary logs?**
A: `PURGE BINARY LOGS TO 'log-bin.000025';`

**Q: How to find out which log file a slave is reading?**
A: `SHOW SLAVE STATUS \G;`

**Q: Where are the logs stored by default?**
A: In the MySQL data directory (e.g., `/var/lib/mysql`)

**Q: How to monitor query performance in real-time?**
A: Use `performance_schema` or tools like MySQL Enterprise Monitor.

---

## 34. Replication (451–460)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is replication in MySQL?**
A: The process of copying data from one MySQL server (master) to another (slave).

**Q: Types of replication in MySQL?**
A: Statement-based, row-based, and mixed.

**Q: What is GTID-based replication?**
A: Uses Global Transaction IDs to track transactions for reliable replication.

**Q: How to start replication?**
A: Configure master and slave with binary logging and replication users.

**Q: How to check replication status?**
A: `SHOW SLAVE STATUS \G`

**Q: What is the use of CHANGE MASTER TO?**
A: To configure a slave's replication source.

**Q: How to stop/start replication?**
A: `STOP SLAVE;`
   `START SLAVE;`

**Q: What does Seconds_Behind_Master mean?**
A: How far the slave is behind the master in seconds.

**Q: Can you replicate from multiple masters?**
A: Yes, using multi-source replication (MySQL 5.7+).

**Q: How to skip a problematic replication query?**
A: `SET GLOBAL SQL_SLAVE_SKIP_COUNTER = 1; START SLAVE;`

---

## 35. Events (Specific Range Missing)

**Q: What is an event in MySQL?**
A: A scheduled task that runs SQL statements at a specific time.

**Q: How to enable the event scheduler?**
A: `SET GLOBAL event_scheduler = ON;`

**Q: How to create an event?**
A:
```sql
CREATE EVENT my_event
ON SCHEDULE EVERY 1 HOUR
DO
UPDATE table SET column = value;
```

**Q: How to drop an event?**
A: `DROP EVENT event_name;`

**Q: Can events be recurring?**
A: Yes, use EVERY in the schedule clause.

**Q: How to disable an event temporarily?**
A: `ALTER EVENT event_name DISABLE;`

**Q: Where are events stored?**
A: In `information_schema.EVENTS`.

**Q: How to list all events?**
A: `SHOW EVENTS;`

**Q: Can an event call a stored procedure?**
A: Yes.

**Q: What happens if the event scheduler is OFF?**
A: Events will not execute.

---

## 36. Troubleshooting (Specific Range Missing)

**Q: What causes the "Too many connections" error?**
A: Exceeding `max_connections` limit.

**Q: How to fix table corruption errors?**
A: Use `REPAIR TABLE table_name;`

**Q: What does "Lock wait timeout exceeded" mean?**
A: A transaction couldn't obtain a lock in the given time.

**Q: How to resolve a deadlock?**
A: Analyze with `SHOW ENGINE INNODB STATUS` and optimize transactions.

**Q: What causes "Table doesn't exist" error even though it does?**
A: Case sensitivity issues on case-sensitive filesystems (e.g., Linux).

**Q: What to do when MySQL crashes frequently?**
A: Check logs, update server version, check hardware and config.

**Q: What is the "Out of memory" error in MySQL?**
A: MySQL tried to use more memory than the OS allowed.

**Q: What is "MySQL has gone away"?**
A: Connection lost due to timeout or packet size.

**Q: What is the default maximum packet size in MySQL?**
A: 4MB (`max_allowed_packet`)

**Q: How to fix character encoding issues?**
A: Ensure consistent CHARSET and COLLATION across DB, tables, and connections.

---

## 37. User Management (Specific Range Missing)

*(Note: This section seems duplicated. Review required.)*

**Q: How do you create a new MySQL user?**
A: `CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';`

**Q: How to grant privileges to a user?**
A: `GRANT SELECT, INSERT ON database.* TO 'username'@'localhost';`

**Q: How to revoke privileges?**
A: `REVOKE SELECT, INSERT ON database.* FROM 'username'@'localhost';`

**Q: How to delete a MySQL user?**
A: `DROP USER 'username'@'localhost';`

**Q: How to view all MySQL users?**
A: `SELECT User, Host FROM mysql.user;`

**Q: What does WITH GRANT OPTION do?**
A: Allows the user to grant their privileges to others.

**Q: How to change a user password?**
A: `ALTER USER 'username'@'localhost' IDENTIFIED BY 'newpassword';`

**Q: How to enforce SSL connections?**
A: Grant privileges with REQUIRE SSL.

**Q: How to block remote root login?**
A: Ensure root is only allowed from `localhost`.

**Q: How to list user privileges?**
A: `SHOW GRANTS FOR 'username'@'host';`

---

## 38. Advanced Indexing & Query Optimization (Specific Range Missing)

**Q: What is a covering index?**
A: An index that contains all the columns needed by a query.

**Q: What is the difference between clustered and non-clustered indexes?**
A: InnoDB's primary key is clustered; other indexes are non-clustered.

**Q: How does index selectivity affect performance?**
A: Higher selectivity (more unique values) improves performance.

**Q: What is a full table scan?**
A: Reading every row in the table due to no usable index.

**Q: How to avoid using SELECT *?**
A: Always specify columns — it's better for performance and clarity.

**Q: What is an execution plan?**
A: The strategy MySQL uses to execute a query.

**Q: How to reduce temporary tables on disk?**
A: Use smaller result sets and avoid large text/BLOB fields in sorts.

**Q: Why use LIMIT in subqueries?**
A: It can reduce the number of rows scanned and improve speed.

**Q: What is the derived_merge optimization?**
A: Merges derived tables into the outer query for efficiency (MySQL 5.7+).

**Q: Why should you avoid functions on indexed columns in WHERE?**
A: It disables index usage.

---

## 39. Backup and Recovery (Specific Range Missing)

**Q: How to back up a MySQL database?**
A: Use mysqldump:
```bash
mysqldump -u root -p database_name > backup.sql
```

**Q: How to restore a MySQL database?**
A:
```bash
mysql -u root -p database_name < backup.sql
```

**Q: How to backup all databases?**
A:
```bash
mysqldump -u root -p --all-databases > all_backup.sql
```

**Q: How to backup only table structure?**
A:
```bash
mysqldump -d -u root -p dbname > structure.sql
```

**Q: How to backup specific tables?**
A:
```bash
mysqldump -u root -p dbname table1 table2 > tables.sql
```

**Q: What is the difference between logical and physical backup?**
A: Logical: SQL text (e.g., mysqldump). Physical: binary files (e.g., mysqlhotcopy).

**Q: What is mysqlpump?**
A: A newer parallel dump tool introduced in MySQL 5.7.

**Q: Can you compress a backup?**
A: Yes, with tools like gzip:
```bash
mysqldump dbname | gzip > dbname.sql.gz
```

**Q: How to restore a gzipped backup?**
A:
```bash
gunzip < dbname.sql.gz | mysql -u root -p dbname
```

**Q: How to backup triggers and routines?**
A: Use `--routines --triggers` with `mysqldump`.

---

## 40. Migration & Compatibility (Specific Range Missing)

**Q: How to migrate from MySQL to PostgreSQL?**
A: Use tools like pgloader, or export/import via scripts.

**Q: What is MySQL Workbench used for?**
A: Visual database design, query execution, server management, and migration.

**Q: How to check the MySQL version?**
A: `SELECT VERSION();`

**Q: How to ensure compatibility between versions?**
A: Review the MySQL Release Notes and test with staging.

**Q: How to convert MyISAM to InnoDB?**
A: `ALTER TABLE table_name ENGINE=InnoDB;`

**Q: Can you downgrade MySQL safely?**
A: It's risky; backup data and test before attempting.

**Q: How to migrate data from Excel to MySQL?**
A: Export Excel to CSV → use `LOAD DATA INFILE` or import via Workbench.

**Q: What is a .frm file?**
A: Stores table structure (used in older MySQL versions).

**Q: What is the alternative to mysqldump for large datasets?**
A: `mysqlpump`, Percona XtraBackup, or physical backup.

**Q: How to migrate between MySQL and MariaDB?**
A: Generally compatible, but test features and engine support.

---

## 41. Miscellaneous (391–400)

**Q: What is information_schema?**
A: A virtual database providing metadata about other databases.

**Q: What is performance_schema?**
A: A tool to monitor performance and query metrics.

**Q: What are storage engines in MySQL?**
A: Pluggable modules like InnoDB, MyISAM, MEMORY, etc.

**Q: How to change the storage engine of a table?**
A: `ALTER TABLE table_name ENGINE = InnoDB;`

**Q: What is sql_mode?**
A: Determines SQL behavior (e.g., strict mode, ANSI mode).

**Q: How to set SQL mode?**
A: `SET GLOBAL sql_mode = 'STRICT_ALL_TABLES';`

**Q: How to disable foreign key checks temporarily?**
A: `SET FOREIGN_KEY_CHECKS = 0;`

**Q: What is auto_increment_offset?**
A: Sets the starting value of AUTO_INCREMENT fields in replication.

**Q: How to show warnings after a query?**
A: `SHOW WARNINGS;`

**Q: How to find duplicate rows in a table?**
A: `SELECT col, COUNT(*) FROM table GROUP BY col HAVING COUNT(*) > 1;`

---

## 42. Transactions & Isolation (401–410)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is a transaction in MySQL?**
A: A sequence of one or more SQL operations treated as a single logical unit of work.

**Q: What are the ACID properties?**
A: Atomicity, Consistency, Isolation, Durability.

**Q: How to start a transaction?**
A: `START TRANSACTION;`

**Q: How to commit a transaction?**
A: `COMMIT;`

**Q: How to rollback a transaction?**
A: `ROLLBACK;`

**Q: What is the default isolation level in MySQL?**
A: REPEATABLE READ.

**Q: What are the isolation levels in MySQL?**
A: READ UNCOMMITTED, READ COMMITTED, REPEATABLE READ, SERIALIZABLE.

**Q: What is dirty read?**
A: Reading uncommitted changes of another transaction.

**Q: What is a phantom read?**
A: Getting different results when re-running the same query due to concurrent inserts.

**Q: How to set the isolation level?**
A: `SET SESSION TRANSACTION ISOLATION LEVEL READ COMMITTED;`

---

## 43. JSON in MySQL (411–420)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: Does MySQL support JSON data type?**
A: Yes, from MySQL 5.7+.

**Q: How to create a column with JSON data type?**
A: `CREATE TABLE t (data JSON);`

**Q: How to insert JSON data?**
A: `INSERT INTO t (data) VALUES ('{"name": "Rakesh", "age": 30}');`

**Q: How to extract data from a JSON column?**
A: `SELECT data->'$.name' FROM t;`

**Q: How to get all keys in a JSON object?**
A: `SELECT JSON_KEYS(data) FROM t;`

**Q: How to validate JSON format in MySQL?**
A: Use `JSON_VALID()` function.

**Q: How to modify a value in JSON?**
A: `SELECT JSON_SET(data, '$.name', 'Amit') FROM t;`

**Q: How to remove a key from JSON?**
A: `SELECT JSON_REMOVE(data, '$.age') FROM t;`

**Q: Can you index JSON data in MySQL?**
A: Only with generated columns and indexes on them.

**Q: How to search inside JSON array?**
A: `SELECT * FROM t WHERE JSON_CONTAINS(data->'$.tags', '["mysql"]');`

---

## 44. Views (421–430)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is a view in MySQL?**
A: A virtual table based on a SQL SELECT statement.

**Q: How to create a view?**
A: `CREATE VIEW v1 AS SELECT name FROM users WHERE age > 18;`

**Q: How to drop a view?**
A: `DROP VIEW view_name;`

**Q: Can a view be updated?**
A: Yes, if it's a simple SELECT without JOINs or aggregates.

**Q: How to see view definition?**
A: `SHOW CREATE VIEW view_name;`

**Q: Can views be indexed?**
A: No, but queries on views can use base table indexes.

**Q: What is a materialized view?**
A: A view that stores actual data (not supported natively in MySQL).

**Q: Can views use parameters?**
A: No. Use stored procedures or functions instead.

**Q: Can a view join multiple tables?**
A: Yes.

**Q: How to replace a view definition?**
A: `CREATE OR REPLACE VIEW view_name AS SELECT ...;`

---

## 45. Stored Routines & Functions (431–440)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is a stored procedure?**
A: A reusable block of SQL logic stored in the database.

**Q: How to create a stored procedure?**
A:
```sql
DELIMITER $$
CREATE PROCEDURE testproc()
BEGIN
  SELECT NOW();
END$$
DELIMITER ;
```

**Q: How to call a stored procedure?**
A: `CALL testproc();`

**Q: How to drop a stored procedure?**
A: `DROP PROCEDURE testproc;`

**Q: What is the difference between a procedure and a function?**
A: A function returns a value and can be used in SQL expressions.

**Q: How to create a function?**
A: `CREATE FUNCTION getYear() RETURNS INT RETURN YEAR(CURDATE());`

**Q: What are IN, OUT, INOUT parameters?**
A: Control how data is passed to/from stored procedures.

**Q: How to list all stored procedures?**
A: `SHOW PROCEDURE STATUS;`

**Q: Can stored procedures call other procedures?**
A: Yes.

**Q: How to debug stored procedures?**
A: Use SELECTs inside the procedure or use Workbench's debugger.

---

## 46. Partitioning (441–450)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is table partitioning?**
A: Dividing a table into multiple pieces for performance/scalability.

**Q: What types of partitioning are available in MySQL?**
A: RANGE, LIST, HASH, KEY.

**Q: How to create a partitioned table?**
A:
```sql
CREATE TABLE sales (
  id INT, sale_date DATE
)
PARTITION BY RANGE (YEAR(sale_date)) (
  PARTITION p2023 VALUES LESS THAN (2024),
  PARTITION p2024 VALUES LESS THAN (2025)
);
```

**Q: Can you add partitions later?**
A: Yes, with ALTER TABLE.

**Q: Can a partitioned table have a foreign key?**
A: No, MySQL does not allow foreign keys on partitioned tables.

**Q: Can we create indexes on partitions?**
A: Yes, but they apply to the whole table, not individual partitions.

**Q: How to check table partitions?**
A: `SELECT * FROM information_schema.PARTITIONS WHERE TABLE_NAME = 'sales';`

**Q: What is subpartitioning?**
A: Partitioning within a partition (MySQL supports limited subpartitioning).

**Q: Can you remove a partition?**
A: Yes, using `ALTER TABLE ... DROP PARTITION`.

**Q: What is the performance benefit of partitioning?**
A: Allows MySQL to scan only relevant partitions, reducing I/O.

---

## 47. Replication & High Availability (451–460)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is MySQL replication?**
A: It allows data from one server (master) to be replicated to one or more (slave) servers.

**Q: What types of replication are supported?**
A: Statement-based, row-based, and mixed.

**Q: How to enable binary logging for replication?**
A: Add `log-bin=mysql-bin` in the MySQL config file.

**Q: What is GTID-based replication?**
A: Uses Global Transaction Identifiers for better consistency and recovery.

**Q: How to check replication status?**
A: `SHOW SLAVE STATUS\G`

**Q: What is semi-synchronous replication?**
A: The master waits for at least one slave to acknowledge the transaction.

**Q: What is the role of relay-log?**
A: Stores the master's binary log events on the slave.

**Q: What causes replication lag?**
A: Network issues, slow queries on the slave, or high load on master.

**Q: Can you replicate between different versions of MySQL?**
A: Yes, but the slave must not be older than the master.

**Q: How to skip a problematic replication query?**
A: `SET GLOBAL SQL_SLAVE_SKIP_COUNTER = 1; START SLAVE;`

---

## 48. MySQL Cluster & Scaling (461–470)

**Q: What is MySQL Cluster?**
A: A high-availability, auto-sharded version of MySQL using NDB storage engine.

**Q: What is sharding?**
A: Splitting data across multiple servers to scale horizontally.

**Q: What are MySQL Fabric and ProxySQL used for?**
A: High availability, load balancing, and sharding management.

**Q: What is Galera Cluster?**
A: A synchronous multi-master cluster solution for MySQL.

**Q: What is a data node in MySQL Cluster?**
A: A node that stores the actual data in NDB.

**Q: What is a management node in MySQL Cluster?**
A: Coordinates cluster startup and configuration.

**Q: What are read/write split proxies?**
A: Tools that route read queries to replicas and write queries to master.

**Q: What is load balancing in MySQL?**
A: Distributing traffic among multiple database nodes to increase performance.

**Q: Can clustering and replication be combined?**
A: Yes, often used in large-scale architectures.

**Q: What are the challenges of clustering?**
A: Configuration complexity, data consistency, and conflict resolution.

---

## 49. Performance Tuning (471–480)

*(Note: This section seems duplicated/overlapping. Review required.)*

**Q: What is the slow query log?**
A: Logs queries that exceed a time threshold.

**Q: How to enable the slow query log?**
A: `SET GLOBAL slow_query_log = 1;`

**Q: What is EXPLAIN used for?**
A: Analyzing how MySQL executes a query.

**Q: How to check index usage?**
A: Use EXPLAIN and observe the `key` column.

**Q: What are some common tuning parameters?**
A: `innodb_buffer_pool_size`, `query_cache_size`, `max_connections`, `tmp_table_size`.

**Q: What is innodb_buffer_pool_size?**
A: Memory allocated for caching InnoDB data and indexes.

**Q: What is query cache?**
A: Caches SELECT results (deprecated in MySQL 8.0).

**Q: How to identify performance bottlenecks?**
A: Use slow logs, `performance_schema`, and monitoring tools.

**Q: What is mysqltuner?**
A: A Perl script that gives performance tuning suggestions.

**Q: How to reduce locking issues?**
A: Use shorter transactions, proper indexes, and avoid full-table scans.

---

## 50. Monitoring & Maintenance (481–490)

**Q: What is MySQL Enterprise Monitor?**
A: A commercial tool for monitoring MySQL performance and health.

**Q: What is performance_schema?**
A: Collects data on query execution, memory usage, and threads.

**Q: How to monitor disk space used by a database?**
A:
```sql
SELECT table_schema AS "DB", SUM(data_length + index_length)/1024/1024 AS "Size MB"
FROM information_schema.tables GROUP BY table_schema;
```

**Q: How to check long-running queries?**
A: `SHOW PROCESSLIST;`

**Q: What is OPTIMIZE TABLE used for?**
A: Reorganizes the table and defragments data.

**Q: How to automate backups?**
A: Use cron jobs or scheduled tasks with scripts.

**Q: What is ANALYZE TABLE used for?**
A: Updates index statistics to optimize query planning.

**Q: What does CHECK TABLE do?**
A: Verifies table integrity.

**Q: How often should you monitor your database?**
A: Continuously, using monitoring dashboards and alerts.

**Q: What are good MySQL monitoring tools?**
A: Percona Monitoring and Management, MySQL Workbench, Nagios, Zabbix.

---

## 51. Advanced & Scenario-Based (491–500)

**Q: What happens if a transaction fails midway?**
A: It rolls back automatically if not committed.

**Q: What is a deadlock?**
A: Two transactions waiting on each other's locked resources.

**Q: How to detect deadlocks?**
A: Use: `SHOW ENGINE INNODB STATUS;`

**Q: How to resolve deadlocks?**
A: Reorder queries, shorten transactions, or retry logic.

**Q: How to enforce case sensitivity in MySQL?**
A: Use a binary collation like `utf8mb4_bin`.

**Q: How to store time zone-aware timestamps?**
A: Use TIMESTAMP type and configure session time zones.

**Q: How to prevent SQL injection in MySQL apps?**
A: Use prepared statements and ORM libraries.

**Q: What is the max size of a MySQL table?**
A: Depends on the storage engine and OS, but InnoDB can handle terabytes.

**Q: How to handle millions of rows efficiently?**
A: Use indexing, partitioning, and optimized queries.

**Q: What's your MySQL troubleshooting workflow?**
A: Check error logs → `SHOW PROCESSLIST` → slow log → `EXPLAIN` → configs → monitor resources.

---

## 🎯 Usage

Use this repo to:
- Prepare for MySQL interviews.
- Strengthen your SQL knowledge.
- Build SQL-based tutorials or vlogs.

## 📢 Contributing

Want to add more questions or fix something? Feel free to contribute via pull request.

## ⭐ Support

If this repo helped you, give it a ⭐ and share it with others!

---

Created by [Rakesh Singh Bajetha](https://github.com/your-profile) for the **Edubrotech** YouTube channel.

> "Knowledge shared is knowledge squared!" 🚀
