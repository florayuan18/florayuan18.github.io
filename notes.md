---
layout: page
title: Tech Talk Notes
subtitle:
---
# Tech Talk 1 - Linked Lists Part 2
Linked Lists:
* [Tri 2 Tech Talk](https://github.com/nighthawkcoders/nighthawk_csa/wiki/Tri-2:-Tech-Talk-8:-Linked-Lists,-Queues,-Stacks)
* Array is a data structure
* Linked Lists and Stacks and Queues are next

Challenges:
* Managing data (nodes) in structure
* Implementing generic data and ForEach loop support
* [Generic T and Iterable Interface](https://www.geeksforgeeks.org/java-implementing-iterator-and-iterable-interface/)
* Generic T
> Don't want to reimplement it multiple times
> Generic - don't have to put in type
* Iterable Interface
> Similar to extends
> Typically has no code, just the abstract interface

Challenges:
* Using Iterable to train the enhanced for loop - navigating the data structure

Challenge 1:
* In-queue - adding someone to the line (push) - add
* De-queue - removing someone from the line (pop) - remove
* Stack - using the terms push and pop
* In-queue | push | add
* De-queue | pop | remove
* Keep track of head and tail of the queue
* Queue has linked list that makes these connections
* Head remains constant when queue-ing
* Tail remains constant when de-queue-ing (remove from head)

Challenge 2:
* Ordered queues
* Dequeue the two queues
* Use "peek" that looks at the queue and returns the data

Challenge 3:
* Build a queue 
* Example [without Generic T and Iterable](https://github.com/nighthawkcoders/nighthawk_csa/blob/master/src/main/java/com/nighthawk/csa/utility/LinkedLists/Stack.java)
* Load up the queue and print it
* De-queue the elements and push into the stack - reverse the results
* public class Queue<T> implements Iterable<T> { LinkedList<T> head, tail;
> T means that it's generic data
* Queue has a linked list - queue is a data structure itself
* Linked list has data
* Nil = nothing/null
* Middle is nothing - cannot get middle property without de-queueing
* Iterating - Queue Iterator
> Null = done with the loop
> tell the iterator where to start from

# Tech Talk 0 - Data Structures

Data Structures Definition:
* Method of organizing
* Single integer values
* Help programmers build what they want
* Optimized and efficient code
  ![](https://www.tutorialscan.com/wp-content/uploads/2018/11/Data-Structure-Types.png)

Programming Paradigms:
* Imperative
> Uses statements to change program's state
> "how" the program works
> Procedural programming - type that has one or more procedures
> Maintains quality
* Object-Oriented
> Uses classes and objects
> Structure software to reusable blueprints
> Define classes, protect information, extend classes, create subclass behavior

Data Structures Example:
* Arrays/Lists
* Dictionaries/HashMaps

Challenges:
* Create alternate menu with data structure
* Swap numbers and add to Menu
* Matrix