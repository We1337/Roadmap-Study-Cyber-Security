The DROP statement in SQL is used to delete objects, such as tables, views, indexes, and procedures from a database. The basic syntax of the DROP statement is as follows:

```sql
DROP object_type object_name;
```

Here, `object_type` is the type of object that you want to delete, such as TABLE, VIEW, INDEX, or PROCEDURE. `object_name` is the name of the object that you want to delete.

For example, to delete a table called `employees`, you would use the following DROP statement:

```sql
DROP TABLE employees;
```

This statement will delete the `employees` table and all of its associated data. Note that once you delete a table or other object, you cannot undo the deletion.

You can also use the DROP statement to delete other types of objects. For example, to delete a view called `sales_report`, you would use the following statement:

```sql
DROP VIEW sales_report;
```

To delete an index called `idx_employee_salary`, you would use the following statement:

```sql
DROP INDEX idx_employee_salary;
```

And to delete a stored procedure called `get_employee_info`, you would use the following statement:

```sql
DROP PROCEDURE get_employee_info;
```

In general, you should be careful when using the DROP statement, as it permanently deletes data and cannot be undone. It's a good practice to back up your database before making any changes to your schema.