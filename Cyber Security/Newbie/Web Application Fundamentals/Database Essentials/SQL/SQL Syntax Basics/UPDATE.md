The UPDATE statement in SQL is used to modify existing rows of data in a table. The basic syntax of the UPDATE statement is as follows:

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

Here, `table_name` is the name of the table that you want to update data in. The `SET` clause specifies the columns that you want to update and the new values that you want to set for each column. The `WHERE` clause specifies which rows to update based on a given condition.

For example, let's say you have a table called `employees` with the following columns: `id`, `name`, `title`, and `salary`. To update the salary of an employee with a certain `id`, you would use the following UPDATE statement:

```sql
UPDATE employees
SET salary = 50000
WHERE id = 123;
```

This statement will update the `salary` column of the employee with `id` 123 to 50000. Note that the `WHERE` clause is used to specify which row(s) to update. In this case, only the row with `id` 123 will be updated.

You can also use the UPDATE statement to update multiple columns at once. For example:

```sql
UPDATE employees
SET title = 'Manager', salary = 60000
WHERE id = 123;
```

This statement will update both the `title` and `salary` columns of the employee with `id` 123.

Finally, you can also use the UPDATE statement to update data in a table using a subquery. For example:

```sql
UPDATE employees
SET salary = salary * 1.1
WHERE id IN (
    SELECT id
    FROM performance_reviews
    WHERE rating = 'Excellent'
);
```

This statement will update the `salary` column of all employees whose `id` appears in the subquery, which selects `id` values from a table called `performance_reviews` where the rating is "Excellent". The `SET` clause multiplies each employee's salary by 1.1, increasing it by 10%.