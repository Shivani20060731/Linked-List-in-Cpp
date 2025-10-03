# Linked-List-in-Cpp
Implementation of Linked List in C++

Aim

To study and implement the concept of Linked Lists in C++ using dynamic memory allocation and pointer-based connectivity.


Software Used

Online C/C++ Compiler


Theory

A Linked List is a dynamic data structure that consists of a sequence of nodes. Each node contains:

1. Data field – to store the actual value.


2. Pointer field – to store the address of the next node in the sequence.



Unlike arrays, linked lists do not require contiguous memory allocation. Nodes are created dynamically in the heap, and their addresses are stored in the pointer fields, thereby linking them together.

Types of Linked Lists:

Singly Linked List – each node points to the next node, last node points to NULL.

Doubly Linked List – each node has two pointers: one pointing to the next node and another to the previous node.

Circular Linked List – last node points back to the first node, forming a cycle.


In this experiment, we will focus on Singly Linked Lists with two examples:

1. Basic Node Creation and Linking


2. Linked List with Head Insertion


Part A: Linked List Node Implementation

Explanation with Code Theory

This program demonstrates the creation of a basic linked structure using a Node class.

Each node holds an integer value and a pointer to the next node.

Two nodes are dynamically allocated using new.

The first node is linked to the second by updating the next pointer.

A display() function is used to print the node’s data and linkage status.


This introduces the fundamental principle of linked lists: pointer-based connectivity.

Algorithm

1. Define a Node class containing:

An integer data

A pointer next



2. Dynamically allocate two nodes using new.


3. Assign values to the nodes.


4. Set the next of the first node to point to the second node.


5. Set the next of the second node to NULL.


6. Traverse using display() to print each node’s content.


7. End.


Part B: Simple Linked List with Head Insertion

Explanation with Code Theory

This program extends the idea by building a linked list through head insertion.

The addToFront() function inserts new nodes at the beginning.

The head pointer is updated to always point to the newest node.

printList() traverses the list and prints all values until NULL.


Time Complexity: Insertion at head is O(1), which is efficient compared to shifting elements in arrays.

This approach simulates stack-like behavior, where the most recent element is always at the front.


Algorithm

1. Define a Node class with data and next pointer.


2. Initialize head = nullptr.


3. For each new element:

Dynamically create a new node.

Set its next pointer to the current head.

Update head to point to the new node.



4. Traverse using printList() to display values until NULL.


5. End.


Conclusion

The experiments demonstrate how singly linked lists are implemented in C++ using classes and dynamic memory.

Part A (Two-Node Implementation): Introduces the basic concept of node creation, memory allocation, and pointer-based linkage.

Part B (Head Insertion): Extends the concept to support efficient insertion, traversal, and modular function design.
