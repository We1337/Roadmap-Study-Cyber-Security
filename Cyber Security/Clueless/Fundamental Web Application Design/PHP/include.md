In PHP, the `include` statement is used to include and execute the contents of another PHP file in the current PHP script. This can be useful for reusing code across multiple scripts, or for breaking up a large PHP file into smaller, more manageable pieces.

The basic syntax for the `include` statement is as follows:

```php
include 'filename.php'
```

Here, `filename.php` is the name of the file to be included. The `.php` file extension is optional, but it is a common convention for PHP files.

The `include` statement works by inserting the contents of the specified file at the point where it is included in the current script. This means that any PHP code or output in the included file will be executed or displayed in the context of the current script.

It's important to note that if the file specified by `include` cannot be found, PHP will produce a warning message but will continue executing the script. If the `require` statement is used instead of `include`, PHP will produce a fatal error and stop executing the script if the specified file cannot be found.

Here is an example of how to use the `include` statement to include a PHP file in a script:

```php
<?php
// Include a PHP file
include 'header.php';

// Display some content
echo 'This is the main content of the page.';

// Include another PHP file
include 'footer.php';
?>
```

In this example, the `header.php` and `footer.php` files contain code that is reused across multiple pages, such as HTML markup, navigation menus, or other common elements. By using the `include` statement, we can avoid duplicating this code in every PHP file and instead maintain it in a separate file for easier management and maintenance.