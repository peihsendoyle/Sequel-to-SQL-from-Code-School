# Sequel-to-SQL-from-Code-School
http://campus.codeschool.com/courses/the-sequel-to-sql

***Find:***

```SELECT column FROM table 
WHERE criteria AND/OR criteria 
ODER BY ASC/DESC;```

SELECT *: select all the columns in table.

***Insert:***

`INSERT INTO table (column) VALUES (value);`

***Update:***

`UPDATE table SET column = value WHERE criteria;`

***Delete:***

`DELETE FROM table WHERE criteria;`

***Create database:***

`CREATE DATABASE name;`

***Delete database:***

`DROP DATABASE name;`

***Create table:***

```CREATE TABLE name ( 
    column_name1 datatype CONSTRAINT1 CONSTRAINT2, 
    column_name2 datatype CONSTRAINTS,...
    CONSTRAINT name CONSTRAINT_NAME (column, column...
);```

**Constraints:** NOT NULL, UNIQUE, PRIMARY KEY, FOREIGN KEY (REFERENCES table(column) ), CHECK (criteria), DEFAULT.

***Create table:***

**Datatypes:** int, varchar(n), character(n), binary(n), boolean, bigint, decimal(p,s), numeric(p,s), float(p), real, date, time, array, multiset, xml, interval, timestamp...

***Delete table:***

`DROP TABLE name;`

***Add a new column for table:***

`ALTER TABLE name ADD COLUMN name datatype;`

***Delete a column of table:***

`ALTER TABLE table DROP COLUMN column`

***Common aggregate functions:***

`SELECT aggregate_function(column) FROM table;`

**Aggregate functions:** count, sum, avg, min, max...

***Aggregate functions within clause:***

```SELECT column, aggregate_function(column) 
FROM table 
WHERE criteria 
GROUP BY column 
HAVING aggregate_function(column) criteria;```


