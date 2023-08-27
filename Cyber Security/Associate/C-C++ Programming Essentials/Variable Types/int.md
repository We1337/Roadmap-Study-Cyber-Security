In C++, `int` is a fundamental data type used to represent whole numbers, both positive and negative. It stands for "integer." Here's some information about the `int` data type in C++:

- **Syntax**: The syntax for declaring an `int` variable is as follows:
  ```cpp
  int myInteger;
  ```

- **Range**: The range of values that an `int` can represent depends on the platform and the compiler, but it's typically around -2 billion to +2 billion on 32-bit systems and much larger on 64-bit systems.

- **Size**: The size of an `int` varies depending on the system architecture and compiler. On most platforms, it's usually 4 bytes (32 bits), but it can be different on certain architectures.

- **Initialization**: An `int` variable can be initialized at the time of declaration:
  ```cpp
  int age = 25;
  ```

- **Mathematical Operations**: You can perform various mathematical operations on `int` variables, such as addition, subtraction, multiplication, and division.

Example usage:

```cpp
#include <iostream>

int main() {
    int num1 = 10;
    int num2 = 20;
    int sum = num1 + num2;

    std::cout << "Sum: " << sum << std::endl;

    return 0;
}
```

Keep in mind that using `int` may lead to overflow or underflow if calculations exceed the range of the data type. If you need a larger range, consider using `long long int` or other data types that can represent larger integers.