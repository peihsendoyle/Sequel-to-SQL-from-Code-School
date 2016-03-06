# Sequel-to-SQL-from-Code-School

<a data-flickr-embed="true"  href="https://www.flickr.com/photos/101220285@N04/24333913229/in/datetaken/" title="avatar"><img src="https://farm2.staticflickr.com/1521/24333913229_4cfe7c453d.jpg" width="427" height="427" alt="avatar"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

Director: Tieushinshin

http://campus.codeschool.com/courses/the-sequel-to-sql

***Find:***

```
SELECT column FROM table 
WHERE criteria AND/OR criteria 
ODER BY ASC/DESC;
```

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

```
CREATE TABLE name ( 
    column_name1 datatype CONSTRAINT1 CONSTRAINT2, 
    column_name2 datatype CONSTRAINTS,...
    CONSTRAINT name CONSTRAINT_NAME (column, column...
);
```

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

```
SELECT column, aggregate_function(column) 
FROM table 
WHERE criteria 
GROUP BY column 
HAVING aggregate_function(column) criteria;
```

***Join multiple tables:***

```
SELECT table1.column AS "new name", table2.column AS "new name"... 
FROM table1 
TYPE JOIN table2 
ON table1.id = table2.table1_id 
TYPE JOIN table3 
ON table2.id = table3.table2_id...
WHERE criteria 
ORDER BY table1/2/3.column ORDERTYPE;
```

***Aliasses:***

```
SELECT a.column AS "new name", b.column AS "new name"... 
FROM table1 a
TYPE JOIN table2 b
ON a.id = b.a_id 
TYPE JOIN table3 c
ON b.id = c.b_id...
WHERE criteria 
ORDER BY a/b/c.column ORDERTYPE;
```
**Types of JOIN:** INNER, RIGHT OUTER, LEFT OUTER, FULL OUTER.

***Subqueries:***

```
SELECT aggregate_func(column)
FROM table1
WHERE column IN
(SELECT column
FROM table2
WHERE criteria);
```

***JOIN queries:***

```
SELECT aggregate_func(table.column)
FROM table1
TYPE JOIN table2
ON table1.id = table2.table1_id
WHERE criteria;
```

***Aliasses for JOIN queries:***

```
SELECT aggregate_func(a/b.column)
FROM table1 a
TYPE JOIN table2 b
ON a.id = b.a_id
WHERE criteria;
```

