The DELETE statement in SQL is used to remove one or more rows from a table. The basic syntax of the DELETE statement is as follows:

```sql
DELETE FROM table_name
WHERE condition;
```

Here, `table_name` is the name of the table from which you want to delete data. The `WHERE` clause specifies which rows to delete based on a given condition.

For example, let's say you have a table called `employees` with the following columns: `id`, `name`, `title`, and `salary`. To delete an employee with a certain `id`, you would use the following DELETE statement:

```sql
DELETE FROM employees
WHERE id = 123;
```

This statement will delete the row in the `employees` table where the `id` is 123. Note that the `WHERE` clause is used to specify which row(s) to delete.

You can also use the DELETE statement to delete all rows in a table. For example:

```sql
DELETE FROM employees;
```

This statement will delete all rows in the `employees` table, effectively emptying the table.

Finally, you can also use the DELETE statement to delete data from a table using a subquery. For example:

```sql
DELETE FROM employees
WHERE id IN (
    SELECT id
    FROM performance_reviews
    WHERE rating = 'Poor'
);
```

This statement will delete all employees whose `id` appears in the subquery, which selects `id` values from a table called `performance_reviews` where the rating is "Poor". The `WHERE` clause is used to specify which rows to delete.