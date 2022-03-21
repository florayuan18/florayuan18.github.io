---
layout: page
title: Week 0 - Menu Code Snippets
subtitle: Flora Yuan
---
## Challenges
**Week 0 - Menu**

Challenges:
* Adding and Deleting Elements from Queue
* Merge Queues
* Reverse Queues

## Code Snippets
```javascript
    // delete method
    public void delete()
{
    // if queue is empty, return NULL.
    if (this.head == null)
        return;

    System.out.println("Dequeued data: " + head.getData());

    // store previous head and move head one node ahead
    LinkedList<T> temp = this.head;
    this.head = this.head.getNext();

    // if head becomes NULL, then change tail also as NULL
    if (this.head == null)
        this.tail = null;
}
```

* This snippet of code was the delete function I wrote.  It stores the previous head, moving it one ahead.  I had to experiment with how this function would logically flow.

```javascript
if (element1 != null && element2 != null) { // conditions for if both elements are not null
    if (element1 < element2) { // element in first queue is smaller than the element in the second queue
        mergedQueue.add(element1); // first element added first in this case
        mergedQueue.add(element2);
    }
    else { // if the above does not occur
        mergedQueue.add(element2); // second element added first in this case
        mergedQueue.add(element1);
    }
}
```

* This is part of the merging of the two queues.  It shows how the two queues will be compared in order for the final printed out numbers to be in numerical order.

```javascript
public void reverseQueue(Queue<Integer> queue1) { // taking every element of queue1 out
    for (Integer object : queue1) { // passing element from queue1 to object
        myStack.push(object); // object to myStack, goes in order of number 1 2 3
    }
}
```

* This code snippet takes every element out and passes the elements to the object.  Using the for loop, it will go through each of the three elements and push them into myStack.

## GitHub
[Challenge 1](https://github.com/florayuan18/just-to-suffer/commit/69297ed1075b677b2383d9a315ef4eb24b6fcb1c)
[Challenge 2](https://github.com/florayuan18/just-to-suffer/commit/57f719c9fdadfe3a4c10fe78f77b29401c82f3d2)
[Challenge 3](https://github.com/florayuan18/just-to-suffer/commit/a32457f6af54b1b74a59b9cb6f167de373411995)

## Replit
[Replit](https://replit.com/@florayuan18/DataStructures#Main.java)