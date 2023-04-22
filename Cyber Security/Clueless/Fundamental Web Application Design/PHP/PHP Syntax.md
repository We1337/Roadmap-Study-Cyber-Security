The syntax of PHP is similar to other programming languages, such as C and Java. Here are some basic elements of PHP syntax:

1. Comments: Comments in PHP are used to explain the code or to make it more readable. They can be single-line comments or multi-line comments.

Example:

```php
// This is a single-line comment in PHP

/*
This is a 
multi-line 
comment in PHP
*/
```

2. Variables: Variables in PHP are used to store data, and their names begin with a dollar sign ($). Variables can hold different data types, such as strings, numbers, and arrays.

Example:

```php
$name = "John"; // A string variable
$age = 30; // A number variable
$fruits = array("apple", "banana", "orange"); // An array variable
```

3. Operators: PHP has a wide range of operators, including arithmetic, comparison, logical, and assignment operators.

Example:

```php
$a = 10;
$b = 5;

// Arithmetic operators
$c = $a + $b;
$d = $a - $b;
$e = $a * $b;
$f = $a / $b;

// Comparison operators
if ($a == $b) {
  echo "Equal";
} else {
  echo "Not equal";
}

// Logical operators
if ($a > 0 && $b < 10) {
  echo "Both conditions are true";
}

// Assignment operators
$a += 5; // equivalent to $a = $a + 5
```

4. Functions: Functions in PHP are used to encapsulate a block of code that performs a specific task. PHP has many built-in functions, such as `strlen()` to get the length of a string, and `date()` to get the current date and time.

Example:

```php
function say_hello($name) {
  echo "Hello, " . $name;
}

say_hello("John"); // Output: Hello, John
```

5. Control structures: PHP provides various control structures, such as if/else statements, loops, and switch statements, to control the flow of code execution.

Example:

```php
$num = 5;

if ($num > 0) {
  echo "Positive";
} else if ($num < 0) {
  echo "Negative";
} else {
  echo "Zero";
}

for ($i = 0; $i < 5; $i++) {
  echo $i;
}

switch ($num) {
  case 1:
    echo "One";
    break;
  case 2:
    echo "Two";
    break;
  default:
    echo "Other";
}
```

These are some of the basic elements of PHP syntax, and there are many more features and functions available in PHP that can be used to build powerful and dynamic web applications.