A linked list is a data structure that consists of a sequence of elements called "nodes," where each node holds both a value and a reference (or pointer) to the next node in the sequence. Linked lists are used to represent dynamic collections of data where the size can change during program execution. They are particularly useful when frequent insertion and deletion operations are required, as these operations can be performed with a relatively low time complexity.

There are several types of linked lists, including singly linked lists, doubly linked lists, and circular linked lists. Here's an overview of each type:

1. **Singly Linked List**:
   - Each node contains a value and a pointer/reference to the next node in the sequence.
   - The last node typically points to a special node representing the end of the list (often a null reference).
   - Insertions and deletions at the beginning or end of the list are relatively efficient, but accessing elements by index requires traversing the list from the beginning.

2. **Doubly Linked List**:
   - Each node contains a value, a pointer to the next node, and a pointer to the previous node.
   - The first node's previous pointer and the last node's next pointer typically point to null or a sentinel node.
   - Doubly linked lists allow for more efficient insertion and deletion operations at both ends of the list and support traversal in both directions.

3. **Circular Linked List**:
   - Similar to a singly or doubly linked list, but the last node points back to the first node (or a sentinel node) to form a loop.
   - Circular linked lists are useful in scenarios where you want the list to have no clear beginning or end.

Linked lists have advantages and disadvantages compared to arrays. Advantages include efficient insertions and deletions, as well as dynamic memory allocation. However, linked lists tend to use more memory due to the storage of references, and accessing elements by index is less efficient compared to arrays.

Example of a singly linked list in C++:

```cpp
#include <iostream>

class Node {
public:
    int data;
    Node* next;

    Node(int value) : data(value), next(nullptr) {}
};

class LinkedList {
private:
    Node* head;

public:
    LinkedList() : head(nullptr) {}

    void append(int value) {
        Node* newNode = new Node(value);
        if (!head) {
            head = newNode;
        } else {
            Node* current = head;
            while (current->next) {
                current = current->next;
            }
            current->next = newNode;
        }
    }

    void display() {
        Node* current = head;
        while (current) {
            std::cout << current->data << " ";
            current = current->next;
        }
        std::cout << std::endl;
    }
};

int main() {
    LinkedList list;
    list.append(10);
    list.append(20);
    list.append(30);
    list.display(); // Output: 10 20 30

    return 0;
}
```

This example demonstrates the basic structure of a singly linked list with appending and displaying functionalities. Each node holds an integer value and a pointer to the next node in the sequence.