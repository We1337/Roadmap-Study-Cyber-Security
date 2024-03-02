The `include` function in PHP is used to **insert the content of another file** into the current file during **server-side execution**. It's a way to **modularize your code** and **reuse common elements** across different PHP scripts.

Here's a breakdown of how `include` works:

**Functionality:**

- Takes the **path to the file** you want to include as its argument.
- **Reads the entire content** of the included file.
- **Inserts the content** at the point where the `include` statement is used in the current file.
- **Execution continues** as if the included content was directly written in the current file.

**Example:**

PHP

```php
// header.php file
echo "<h1>This is the header</h1>";

// main.php file
include "header.php";

echo "This is the main content of the page.";
```

In this example:

- `header.php` contains the HTML code for the page header.
- `main.php` includes `header.php` using the `include` statement.
- When the server processes `main.php`, it first reads the content of `header.php` and then inserts it into `main.php` at the point of the `include` statement.
- The final output will be:

HTML

```html
<h1>This is the header</h1>
This is the main content of the page.
```

**Important Points:**

- **File path:** The path to the included file can be relative (relative to the current file) or absolute (starting from the document root).
- **Error handling:** Unlike `require`, `include` will **not generate a fatal error** if the included file is not found. Instead, it will issue a **warning** and continue execution. This means it's essential to check for potential errors using functions like `file_exists` before using `include` to avoid unexpected behavior.
- **Security:** Be cautious when including files from untrusted sources, as it can introduce security vulnerabilities.

**Alternatives:**

- **`require`:** Similar to `include` but throws a **fatal error** if the file is not found. This can be useful for ensuring critical files are always present.
- **`require_once` and `include_once`:** These variations ensure the file is included only **once** within a script, preventing duplicate content from being inserted if the same file is included multiple times.

Overall, `include` is a valuable tool for code reusability and modularity in PHP applications. However, remember to use it judiciously, handle potential errors, and prioritize security when including external files.