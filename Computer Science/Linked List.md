In computer science, a linked list is a data structure that represents a sequence of elements where each element points to the next one in the sequence. A linked list is made up of nodes, each containing a value and a reference to the next node in the list.

Here's an example of a linked list in Python:

```Python
# Define the Node class
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

# Define the LinkedList class
class LinkedList:
    def __init__(self):
        self.head = None
    
    # Method to add a new node to the end of the list
    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
            return
        last_node = self.head
        while last_node.next:
            last_node = last_node.next
        last_node.next = new_node
    
    # Method to add a new node at the beginning of the list
    def prepend(self, data):
        new_node = Node(data)
        new_node.next = self.head
        self.head = new_node
    
    # Method to insert a new node after a specific node in the list
    def insert_after_node(self, prev_node, data):
        if not prev_node:
            print("Previous node is not in the list")
            return
        new_node = Node(data)
        new_node.next = prev_node.next
        prev_node.next = new_node
    
    # Method to print the list
    def print_list(self):
        current_node = self.head
        while current_node:
            print(current_node.data)
            current_node = current_node.next
```

In this example, we define two classes - `Node` and `LinkedList`. The `Node` class represents a single node in the linked list, with a `data` attribute and a `next` attribute that points to the next node in the list. The `LinkedList` class represents the linked list itself, with a `head` attribute that points to the first node in the list.

The `LinkedList` class also has several methods for adding nodes to the list - `append` adds a new node to the end of the list, `prepend` adds a new node to the beginning of the list, and `insert_after_node` inserts a new node after a specific node in the list. Finally, there is a `print_list` method that prints out the elements of the linked list.

Here's an example of how to use the linked list class:

```Python
# Create a new linked list
my_list = LinkedList()

# Add some nodes to the list
my_list.append("A")
my_list.append("B")
my_list.append("C")
my_list.append("D")
my_list.prepend("E")

# Insert a new node after the second node
second_node = my_list.head.next
my_list.insert_after_node(second_node, "F")

# Print the list
my_list.print_list()
```

This code creates a new linked list, adds some nodes to the list using the `append` and `prepend` methods, inserts a new node after the second node using the `insert_after_node` method, and prints out the elements of the linked list using the `print_list` method. The output of the program will be:

```
E
A
B
F
C
D
```