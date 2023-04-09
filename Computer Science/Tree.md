In computer science, a tree is a non-linear data structure that consists of nodes connected by edges or branches. Each node in a tree represents a value or an object, and it can have zero or more child nodes.

In a tree, there is a single node called the root node that has no parent nodes. Every other node in the tree has exactly one parent node, except for the nodes at the bottom of the tree, called the leaf nodes, which have no child nodes.

Here's an example of how to create a simple tree in Python using classes:

```Python
class Node:
    def __init__(self, value):
        self.value = value
        self.children = []

    def add_child(self, child_node):
        self.children.append(child_node)

root = Node(1)
child1 = Node(2)
child2 = Node(3)
root.add_child(child1)
root.add_child(child2)
```

In this example, we define a Node class that has a value and a list of children. We also define a method called add_child that allows us to add child nodes to a node. Finally, we create a root node with a value of 1 and two child nodes with values of 2 and 3, respectively. We add the child nodes to the root node using the add_child method.

[[Binary Tree]]
[[Binary Search Tree]]
[[Full Binary Tree]]
[[Complete Binary Tree]]
[[Balanced Tree]]
[[Unbalanced Tree]]