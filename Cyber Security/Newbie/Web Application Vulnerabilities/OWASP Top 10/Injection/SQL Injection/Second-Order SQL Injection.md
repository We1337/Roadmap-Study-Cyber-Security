Second-order SQL injection, also known as stored SQL injection or persistent SQL injection, is a type of SQL injection attack where the malicious payload is stored in the application's database and executed at a later time. It occurs when user-supplied input is stored in a database and used in a subsequent SQL query without proper validation or sanitization.

Here's how second-order SQL injection typically works:

1.  Identify SQL injection vulnerability: The attacker identifies a web application that is vulnerable to SQL injection. This vulnerability arises when user input is stored in a database and later used in SQL queries without adequate validation or sanitization.
2.  Inject malicious payload: The attacker injects specially crafted SQL code as user input, which gets stored in the application's database. This input is not immediately executed but is saved for later use in subsequent SQL queries.
3.  Application logic triggers the injection: The attacker relies on specific application logic or events to trigger the execution of the stored SQL injection payload. This can happen when the stored input is concatenated into a query, typically during a different user's interaction with the application.
4.  Execution of the stored payload: When the application uses the stored input in a subsequent SQL query without proper validation, the injected SQL code is executed, leading to potential data manipulation, unauthorized access, or other malicious activities.
5.  Exploiting the obtained access or data: Once the injected SQL code is executed, the attacker can exploit the vulnerability to gain unauthorized access, retrieve sensitive data, modify or delete data, or perform other malicious actions.

To protect against second-order SQL injection attacks, developers should implement the following security measures:

1.  Input validation and parameterized queries: Implement strict input validation and use parameterized queries or prepared statements to separate data from query logic. Validate and sanitize user input before storing it in the database and ensure that the stored data is properly handled and validated when used in subsequent queries.
2.  Stored procedure usage: Use stored procedures or parameterized functions provided by the database system, as they can help protect against SQL injection by encapsulating the SQL code and automatically handling parameterization.
3.  Principle of least privilege: Ensure that database accounts used by the application have minimal privileges required to perform their tasks. Restricting permissions helps limit the potential impact of a successful SQL injection attack.
4.  Regular security testing: Conduct regular security testing, including automated vulnerability scans and manual penetration testing, to identify and remediate SQL injection vulnerabilities. Keep the application and associated frameworks up to date with the latest security patches.

By implementing these security measures, developers can significantly reduce the risk of second-order SQL injection attacks and protect the confidentiality and integrity of their application and data.