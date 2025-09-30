# Linked List  

**Name:** Ninad Phatak  
**PRN:** 24070123065  
**Batch:** ENTC A3  

---

## Overview  

A **Linked List** in C++ is a dynamic data structure that stores data elements (nodes) connected through pointers. Unlike arrays, linked lists do not require contiguous memory allocation, making them efficient for insertions and deletions.  

Each **node** in a linked list consists of:  
- **Data**: The value stored in the node.  
- **Pointer (next)**: The address of the next node.  

Types of Linked Lists:  
- **Singly Linked List**: Each node points to the next node.  
- **Doubly Linked List**: Each node points to both next and previous nodes.  
- **Circular Linked List**: The last node points back to the first node.  

In this document, we demonstrate **basic operations on a singly linked list**:  
1. Adding multiple nodes at the end.  
2. Adding multiple nodes at the start.  
3. Creating a single node.  

---

## 1. Add Multiple Nodes at the End of the Linked List  

### Algorithm  
1. Define a `Node` class with `val` and `next` attributes.  
2. Define a `LinkedList` class with `head` initialized to `NULL`.  
3. To insert at the end:  
   - Create a new node.  
   - If the list is empty, assign it to `head`.  
   - Otherwise, traverse to the last node and link it with the new node.  
4. To display the list, traverse from `head` and print each node’s value.  

### Theory  
This program builds a linked list by adding new nodes at the end.  
- The first inserted node becomes the head.  
- Each subsequent node is appended after traversing to the last node.  
- The `display` function prints all elements sequentially.  

### Output  
Linked List: 10 20 30 40

sql
Copy code

---

## 2. Add Multiple Nodes at the Start of the Linked List  

### Algorithm  
1. Define a `Link` class with `data` and `next` attributes.  
2. To insert at the start:  
   - Create a new node.  
   - Make its `next` point to the current head.  
   - Update head to the new node.  
3. To display, start from `head` and traverse through all nodes, printing their values.  

### Theory  
This program demonstrates how to insert nodes at the **beginning** of a linked list.  
- The head pointer is updated with each new insertion.  
- New nodes are always added before the existing nodes, shifting the list forward.  

### Output  
30->NULL
32->30->NULL
35->32->30->NULL

markdown
Copy code

---

## 3. Single Node of the Linked List  

### Algorithm  
1. Define a `Node` class with attributes `val` and `next`.  
2. Create a new node using dynamic memory allocation (`new`).  
3. Assign a value to the node and set `next = NULL`.  
4. Print the value and the pointer of the node.  

### Theory  
This simple program creates a **single node** of a linked list.  
- The node stores a value (`20`) and a `NULL` pointer since it does not link to any other node.  
- This forms the basic building block of linked lists.  

### Output  
20 0
