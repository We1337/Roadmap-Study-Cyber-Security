In computer science, a queue is an abstract data type that represents a collection of elements, with two principal operations: enqueue, which adds an element to the collection, and dequeue, which removes the least recently added element that was not yet removed. It follows the First In, First Out (FIFO) principle.

Here's an example of a queue implemented in Python:

```Python
class Queue:
    def __init__(self):
        self.items = []
    
    def is_empty(self):
        return self.items == []
    
    def enqueue(self, item):
        self.items.append(item)
    
    def dequeue(self):
        if not self.is_empty():
            return self.items.pop(0)
    
    def size(self):
        return len(self.items)
```

In this example, we define a `Queue` class with three methods: `is_empty`, `enqueue`, `dequeue`, and `size`.

The `is_empty` method returns `True` if the queue is empty, and `False` otherwise.

The `enqueue` method adds an element to the back of the queue.

The `dequeue` method removes the element at the front of the queue, and returns it. If the queue is empty, it returns `None`.

The `size` method returns the number of elements in the queue.

Here's an example of how to use the queue class:

```Python
# Create a new queue
my_queue = Queue()

# Add some elements to the queue
my_queue.enqueue("A")
my_queue.enqueue("B")
my_queue.enqueue("C")

# Remove the front element from the queue
my_queue.dequeue()

# Check the size of the queue
print(my_queue.size())  # Output: 2
```

This code creates a new queue, adds some elements to the queue using the `enqueue` method, removes the front element from the queue using the `dequeue` method, and checks the size of the queue using the `size` method. The output of the program will be:

```
2
```