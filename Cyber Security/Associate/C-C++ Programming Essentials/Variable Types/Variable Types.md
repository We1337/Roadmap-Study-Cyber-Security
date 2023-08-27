In C++, variable types are used to define the nature of the data that a variable can hold. C++ provides a range of built-in variable types to accommodate different kinds of data. Here are the most common variable types in C++:

1. **Integer Types**:
   - `int`: Used for storing integers.
   - `short`: Short integer.
   - `long`: Long integer.
   - `long long`: Long long integer (C++11).
2. **Floating-Point Types**:
   - `float`: Single-precision floating-point number.
   - `double`: Double-precision floating-point number.
   - `long double`: Extended-precision floating-point number.
3. **Character Types**:
   - `char`: Single character.
   - `wchar_t`: Wide character.
   - `char16_t`: 16-bit character (C++11).
   - `char32_t`: 32-bit character (C++11).
4. **Boolean Type**:
   - `bool`: Represents true or false values.
5. **Void Type**:
   - `void`: Represents an empty type, commonly used for functions with no return value.
6. **Array Types**:
   - `T[]`: Array of elements of type `T`.
   - `std::array<T, N>`: Fixed-size array (C++11).
   - `std::vector<T>`: Dynamic array (C++98).
7. **Pointer Types**:
   - `T*`: Pointer to an object of type `T`.
8. **Reference Types**:
   - `T&`: Reference to an object of type `T`.
9. **Enum Types**:
   - `enum`: Defines an enumerated type with named integer constants.
10. **Struct and Class Types**:
    - `struct`: Defines a structure, where members are public by default.
    - `class`: Defines a class, where members are private by default.
11. **Union Types**:
    - `union`: Defines a union, where members share the same memory location.
12. **Pointer-to-Member Types**:
    - Used for dealing with pointers to members of classes.
13. **Function Types**:
    - `returnType (parameters)`: Represents a function type.
14. **Type Aliases**:
    - `typedef`: Creates an alias for an existing type.
    - `using`: Alternative syntax for type aliases (C++11).
15. **Auto Type Inference**:
    - `auto`: Allows the compiler to deduce the type based on the initializer (C++11).
16. **nullptr Type**:
    - `nullptr`: Represents a null pointer (C++11).

These are just the core variable types in C++. Modern C++ (C++11 and later) has introduced several new features, including smart pointers, lambda expressions, and more advanced type management capabilities. Always refer to the documentation of the specific version of C++ you're using for the most accurate information.