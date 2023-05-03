SQL (Structured Query Language) is the language used to communicate with relational databases. Here are some basic SQL syntax concepts:

1.  SELECT statement: The SELECT statement is used to retrieve data from one or more tables in a database. The basic syntax is as follows:

```sql
SELECT column1, column2, ...
FROM table_name;
```

This will retrieve all data from the specified columns in the specified table.   
2. WHERE clause: The WHERE clause is used to filter data based on a specified condition. The basic syntax is as follows:

```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

This will retrieve only the data that satisfies the specified condition.
3. INSERT statement: The INSERT statement is used to insert new data into a table. The basic syntax is as follows:

```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

This will insert a new row with the specified values into the specified table.
4. UPDATE statement: The UPDATE statement is used to update existing data in a table. The basic syntax is as follows:

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

This will update the specified columns with the specified values in the rows that satisfy the specified condition.   
5. DELETE statement: The DELETE statement is used to delete data from a table. The basic syntax is as follows:

```sql
DELETE FROM table_name
WHERE condition;
```

This will delete the rows that satisfy the specified condition from the specified table.
6. ORDER BY clause: The ORDER BY clause is used to sort data based on one or more columns. The basic syntax is as follows:

```sql
SELECT column1, column2, ...
FROM table_name
ORDER BY column1 ASC/DESC, column2 ASC/DESC, ...;
```

This will retrieve the specified columns from the specified table, sorted in ascending (ASC) or descending (DESC) order based on the specified columns.    

These are some of the basic SQL syntax concepts. There are many more advanced concepts and commands, but understanding these basic concepts is essential for working with relational databases.