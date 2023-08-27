Smart pointers are a feature in modern programming languages, particularly in C++ (starting from C++11), that help manage memory automatically and safely, reducing the risk of memory leaks and certain types of errors associated with manual memory management using raw pointers. Smart pointers are a form of RAII (Resource Acquisition Is Initialization) that tie the lifespan of dynamically allocated objects to the lifespan of the smart pointer itself.

There are three main types of smart pointers in C++: `std::unique_ptr`, `std::shared_ptr`, and `std::weak_ptr`. Each type of smart pointer serves a different purpose and provides different ownership semantics:

1. **std::unique_ptr**:
   - Represents sole ownership of a dynamically allocated object.
   - Ensures that the object is automatically deleted when the `std::unique_ptr` goes out of scope or is explicitly reset.
   - Supports move semantics, allowing ownership to be transferred to another `std::unique_ptr`.

2. **std::shared_ptr**:
   - Represents shared ownership of a dynamically allocated object.
   - Keeps track of the number of `std::shared_ptr` instances that share ownership of the object.
   - The object is deleted when the last `std::shared_ptr` owning it is destroyed or reset.

3. **std::weak_ptr**:
   - Works in conjunction with `std::shared_ptr`.
   - Provides a non-owning reference to an object managed by `std::shared_ptr`.
   - Allows you to check whether the object is still valid or has been deleted.

Example of using `std::unique_ptr`:

```cpp
#include <iostream>
#include <memory>

int main() {
    std::unique_ptr<int> ptr(new int(42));

    std::cout << *ptr << std::endl; // Access the value using the dereference operator

    // No need to manually delete the object; it's automatically deleted when ptr goes out of scope

    return 0;
}
```

Example of using `std::shared_ptr`:

```cpp
#include <iostream>
#include <memory>

int main() {
    std::shared_ptr<int> ptr1 = std::make_shared<int>(42);
    std::shared_ptr<int> ptr2 = ptr1; // shared ownership

    std::cout << *ptr1 << " " << *ptr2 << std::endl;

    // The object will be deleted when the last shared_ptr owning it is destroyed

    return 0;
}
```

Smart pointers help prevent memory leaks by automatically deallocating memory when it's no longer needed, as well as avoiding issues like double deletion. However, circular references can still lead to memory leaks when using `std::shared_ptr`. When using smart pointers, you should choose the appropriate type based on your ownership requirements to ensure efficient and safe memory management.