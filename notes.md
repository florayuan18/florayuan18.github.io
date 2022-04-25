---
layout: page
title: Tech Talk Notes
subtitle:
---

# Faculty Lecture Notes
1. Unit 1
* Computer programs take data in and manipulate that data
* Manipulation do to specific instructions --> programming
* Primitive Data Types:
> Integers -> int (integer)
> Floating Point Numbers -> double (fraction/decimal)
> int num;
num = 3;
Declare the variable then assign a value to that variable
> double otherNum = 4.0;
Declaring the variable and assigning at the same time
> Types of primitive data is dependent on memory
> Integer -> byte (1), short (2), int (4), long (8)
> Floating Point Numbers -> float (4), double (8)
> Others are char (characters/Unicode encoding/2) and boolean (true/false/1)


2. Unit 2
* older programming was different
* assembler -> converts assembly language program to machine language
* trying to develop further away from the processor
* programming languages: 
> fortran: designed to solve specific programs
> cobol: identification, reports, very specific purpose
* there are many different ways of solving problems
* think of new ways to improve them
* learn how to use it vs knowing everything about how it works --> how is information provided
> knowing how to use it --> able to solve problems
* object-oriented programming --> defining parts and using those parts to solve problems
> creating a model that is useful
> great in development --> multiple people together


# Tech Talk 3 - Sorts
Challenges:
* Sort and Analysis and see which one is most efficient
* Run each sort 12 times on 5000+ elements
* Throw out high and low

Notes:
* Bubble sort, merge sort, insertion sort, selection sort
* Figure out which is most efficient
* Consider time, comparisons, swaps
* Use inheritance/polymorphism to sort
* Stack Overflow :D

# Tech Talk 2 - Calculator
Challenges:
* Calculator class with string with mathematical expressions
* Create an object with a toString that prints output
* Convert the expression into mathematical tokens
* Convert tokens to reverse polish notation (used for calculators)
* In terms of "After thinking about basic anatomy of an expression and RPN algorithm"
> Given term tokenizer and reverse Polish notation

Split Term:
* Define list of operators - put into hashmaps with precedents on them
* Multiplication is a higher precedent than addition
* Separators and operators (separators when you're tokenizing)

Steps:
* Tokenizer: compare character by character
* Separator breaks up the string - breaks up the items
* Multi Character Term - has to be added together
* Walk through with the Debugger
* Term Tokenizer then Reverse Polish Notation
> Shuffle around
> Two operators in stack
> Reverse Polish is so computer knows how to do operator

Example:
* Tokens (list): 1+2*3
* RPN (list): 1 2 3 * +
* Tokens: 1 * 2 + 3
* 1 2 * 3 +

Challenges:
* 2nd challenge: keeping track of operators
* Extra Credit for shunting yard algorithm

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