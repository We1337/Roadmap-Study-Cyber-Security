`phpinfo()` is a built-in PHP function that displays information about the PHP environment and configuration settings. When `phpinfo()` is called, it generates a detailed report of the PHP configuration, including information on installed extensions, server information, and environment variables.

Here is an example of how to use `phpinfo()`:

```php
<?php
// Output PHP information
phpinfo();
?>
```

When this code is executed, it will display a long list of information about the PHP environment in a web page, including:

- PHP version and build date
- System and server information
- Loaded PHP extensions and their versions
- Configuration settings such as `php.ini` values
- Environment variables such as `$_SERVER` and `$_SESSION`

This information can be useful for debugging purposes, as well as for understanding the configuration and capabilities of the PHP installation. However, it's important to be careful when using `phpinfo()` on a production server, as it can expose sensitive information about the server and potentially be used by attackers to exploit vulnerabilities.