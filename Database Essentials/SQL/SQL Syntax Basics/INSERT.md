The INSERT statement in SQL is used to add new rows of data to a table. The basic syntax of the INSERT statement is as follows:

```sql
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
```

Here, `table_name` is the name of the table that you want to insert data into. The `(column1, column2, column3, ...)` specifies the columns that you want to insert data into. The `VALUES (value1, value2, value3, ...)` specifies the values that you want to insert into the corresponding columns.

For example, let's say you have a table called `customers` with the following columns: `id`, `name`, `email`, and `phone`. To add a new customer to the table, you would use the following INSERT statement:

```sql
INSERT INTO customers (name, email, phone)
VALUES ('John Doe', 'johndoe@example.com', '555-1234');
```

This statement will add a new row to the `customers` table with the name "John Doe", email "[johndoe@example.com](mailto:johndoe@example.com)", and phone number "555-1234". Note that the `id` column was not specified in the INSERT statement. If the `id` column is set to auto-increment, the database system will automatically generate a new unique ID for the new row.

You can also use the INSERT statement to insert multiple rows into a table at once by separating each set of values with a comma. For example:

```sql
INSERT INTO customers (name, email, phone)
VALUES ('Jane Doe', 'janedoe@example.com', '555-5678'),
       ('Bob Smith', 'bobsmith@example.com', '555-9876');
```

This statement will add two new rows to the `customers` table, one for "Jane Doe" and one for "Bob Smith". Note that each set of values is enclosed in parentheses and separated by a comma.

Finally, you can also use the INSERT statement to insert data into a table using a subquery. For example:

```sql
INSERT INTO customers (name, email, phone)
SELECT first_name + ' ' + last_name, email_address, phone_number
FROM contacts
WHERE status = 'active';
```

This statement will insert data into the `customers` table by selecting data from the `contacts` table where the status is "active". The subquery selects the `first_name` and `last_name` columns from the `contacts` table, concatenates them together with a space, selects the `email_address` and `phone_number` columns, and then inserts the resulting data into the `name`, `email`, and `phone` columns of the `customers` table.