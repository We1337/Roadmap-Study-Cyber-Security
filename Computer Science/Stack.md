In computer science, a stack is an abstract data type that represents a collection of elements, with two principal operations: push, which adds an element to the collection, and pop, which removes the most recently added element that was not yet removed. It follows the Last In, First Out (LIFO) principle.

Here's an example of a stack implemented in Python:

```Python
class Stack:
    def __init__(self):
        self.items = []
    
    def is_empty(self):
        return self.items == []
    
    def push(self, item):
        self.items.append(item)
    
    def pop(self):
        if not self.is_empty():
            return self.items.pop()
    
    def peek(self):
        if not self.is_empty():
            return self.items[-1]
    
    def size(self):
        return len(self.items)
```

In this example, we define a `Stack` class with four methods: `is_empty`, `push`, `pop`, `peek`, and `size`.

The `is_empty` method returns `True` if the stack is empty, and `False` otherwise.

The `push` method adds an element to the top of the stack.

The `pop` method removes the element at the top of the stack, and returns it. If the stack is empty, it returns `None`.

The `peek` method returns the element at the top of the stack, without removing it. If the stack is empty, it returns `None`.

The `size` method returns the number of elements in the stack.

Here's an example of how to use the stack class:

```Python
# Create a new stack
my_stack = Stack()

# Add some elements to the stack
my_stack.push("A")
my_stack.push("B")
my_stack.push("C")

# Peek at the top element of the stack
print(my_stack.peek())  # Output: "C"

# Remove the top element from the stack
my_stack.pop()

# Check the size of the stack
print(my_stack.size())  # Output: 2
```

This code creates a new stack, adds some elements to the stack using the `push` method, peeks at the top element of the stack using the `peek` method, removes the top element from the stack using the `pop` method, and checks the size of the stack using the `size` method. The output of the program will be:

```
C
2
```