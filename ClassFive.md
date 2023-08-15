# Understanding Linked Lists

## Introduction
Linked lists are fundamental data structures used in computer science and programming. They provide a way to store and organize data efficiently, especially when the size of the data is dynamic. This document aims to provide a comprehensive understanding of linked lists, their types, operations, and their role in algorithm efficiency.

**Types of Linked Lists:**
* Singly - there is only one reference, and the reference points to the Next node in a linked list.
* Doubly - there is a reference to both the Next and Previous node.
* A circular linked list it doesn’t end with a node pointing to a null value. Instead, it has a node that acts as the tail of the list (rather than the conventional head node), and the node after the tail node is the beginning of the list.

**An Analogy: Building a Train of Data**
   - Comparing Linked Lists to a Train
   - Cars (Nodes) and Connections (Pointers)

    **Why Use Linked Lists?**
   - Dynamic Memory Allocation
   - Insertions and Deletions

   **Basic Operations:**
   - Traversing a Linked List
   - Insertion (at the Beginning, Middle, End)
   - Deletion (at the Beginning, Middle, End)

   ## a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element


##  What Is Big O ?
Big O Notation is a way of evaluating the performance of an algorithm.and we can say it is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.

There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.

An O(1) function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm.
An O(n) function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million)
O(n^2) function, which clearly takes exponentially more time and memory the more elements that you have.

The Big O of time for Includes would be O(n). The Big O of space for Includes would be O(1) The Big O of adding node at the bigging would be O(1) The Big O of adding node before would be O(n).