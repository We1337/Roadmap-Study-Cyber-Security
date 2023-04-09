A binary tree is a type of tree data structure in which each node can have at most two children, referred to as the left child and the right child. The left child is always less than or equal to the parent node, and the right child is always greater than the parent node.

Here's an example of how to create a binary tree in Python using classes:

```Python
class Node:
    def __init__(self, data):
        self.left = None
        self.right = None
        self.data = data

    def insert(self, value):
        if self.data:
            if value < self.data:
                if self.left is None:
                    self.left = Node(value)
                else:
                    self.left.insert(value)
            elif value > self.data:
                if self.right is None:
                    self.right = Node(value)
                else:
                    self.right.insert(value)
        else:
            self.data = value

    def print_tree(self):
        if self.left:
            self.left.print_tree()
        print(self.data)
        if self.right:
            self.right.print_tree()

root = Node(5)
root.insert(3)
root.insert(7)
root.insert(1)
root.insert(9)

root.print_tree()
```

In this example, we define a Node class with a left child, right child, and a data value. We also define an insert method that allows us to insert nodes into the binary tree in their appropriate locations. Finally, we define a print_tree method that prints out the nodes of the tree in order.

We create a root node with a data value of 5, and then insert nodes with values of 3, 7, 1, and 9 into the tree. We then call the print_tree method on the root node to print out the nodes of the tree in order. The output should be:

```
1
3
5
7
9
```