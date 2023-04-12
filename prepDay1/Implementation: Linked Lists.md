# Title: Linked Lists in Python

## Introduction: Have you ever played with LEGO blocks? You can stack them up to make a tower, but what if you want to make a long train instead? You can connect each block to the next one, forming a chain. This is similar to how linked lists work in computer science. Linked lists are data structures that allow us to store and manipulate a collection of data in a dynamic way.
---
### Why use linked lists?
#### Linked lists are useful when we don't know in advance how many items we need to store, or when we need to insert or remove elements frequently. Unlike arrays, which have a fixed size and require contiguous memory allocation, linked lists can grow or shrink dynamically, using only the memory they need. This makes them more flexible and efficient for certain operations.
---
### What are linked lists? 
#### A linked list is a sequence of nodes, each containing a value and a pointer to the next node. The first node is called the head, and the last one is the tail, which points to None. Each node is independent and can be added, removed, or modified without affecting the rest of the list. The pointers form the links between the nodes, allowing us to traverse the list from one end to the other, or to access any node by its position.
---
### How to implement linked lists in Python? 
#### To create a linked list in Python, we can define a Node class with two attributes: value and next. The value stores the data, and the next points to the next node. Then, we can define a LinkedList class with two attributes: head and size. The head is a pointer to the first node, and the size is the number of nodes in the list. We can add methods to insert, remove, search, and print nodes, as well as to get the size and check if the list is empty.
---
---

### Vocabulary/Definition List:

Linked List: A data structure that consists of a sequence of nodes, each containing a value and a pointer to the next node.

Node: An element of a linked list that stores a value and a reference to the next node.

Pointer: A reference to an object in memory, used to connect nodes in a linked list.

Head: The first node in a linked list.

Tail: The last node in a linked list, pointing to None.

Size: The number of nodes in a linked list.

Insertion: The process of adding a new node to a linked list.

Removal: The process of deleting a node from a linked list.

Traversal: The process of visiting all nodes in a linked list.

Search: The process of finding a node with a specific value in a linked list.

 

### Here's an example of how to create and manipulate a singly linked list in Python:

### code :-
### Define a Node class that represents a single node in the linked list
class Node:
    def __init__(self, data=None, next=None):
        self.data = data  # Data stored in the node
        self.next = next  # Pointer to the next node (initially set to None)

### Define the LinkedList class that represents the linked list
class LinkedList:
    def __init__(self):
        self.head = None  # Pointer to the first node in the linked list

    # Add a new node to the end of the linked list
    def append(self, data):
        new_node = Node(data)
        if self.head is None:  # If the linked list is empty, set the new node as the head
            self.head = new_node
            return
        last_node = self.head
        while last_node.next is not None:  # Traverse the linked list to find the last node
            last_node = last_node.next
        last_node.next = new_node  # Set the new node as the next node of the last node

    # Add a new node to the beginning of the linked list
    def prepend(self, data):
        new_node = Node(data)
        new_node.next = self.head  # Set the current head as the next node of the new node
        self.head = new_node  # Set the new node as the head of the linked list

    # Insert a new node after a given node
    def insert_after_node(self, prev_node, data):
        if not prev_node:
            print("Previous node is not in the linked list")
            return
        new_node = Node(data)
        new_node.next = prev_node.next
        prev_node.next = new_node

    # Print the linked list
    def print_list(self):
        current_node = self.head
        while current_node is not None:
            print(current_node.data, end=" ")
            current_node = current_node.next
        print()

### Create a linked list and add some nodes
llist = LinkedList()
llist.append("A")
llist.append("B")
llist.append("C")
llist.append("D")

### Print the linked list
llist.print_list()  # Output: A B C D

### Add a new node to the beginning of the linked list
llist.prepend("E")
llist.print_list()  # Output: E A B C D

### Insert a new node after the node with data="B"
node_B = llist.head.next
llist.insert_after_node(node_B, "F")
llist.print_list()  # Output: E A B F C D

## Things I want to know more about : None.