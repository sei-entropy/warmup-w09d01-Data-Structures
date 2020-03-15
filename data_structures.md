# Data Structures

## Arrays
An array is a collection of items stored at contiguous memory locations. The idea is to store multiple items of the same type together. This makes it easier to calculate the position of each element by simply adding an offset to a base value, i.e., the memory location of the first element of the array (generally denoted by the name of the array).

[url](https://www.geeksforgeeks.org/wp-content/uploads/Array-In-C.png)

### operations 
* Traversing: It prints all the array elements one after another.
* Inserting: It adds an element at given index.
* Deleting: It is used to delete an element at given index.
* Searching: It searches for an element(s) using given index or by value.
* Updating: It is used to update an element at given index.

### Big O 
* average
  Θ(n)
 * worst
  O(n)


## Linked List

## Stack 
A stack is a linear data structure used to store a collection of objects.The order may be LIFO(Last In First Out) or FILO(First In Last Out). Items can be added and stored in a stack using a push operation. And can be retrieved using a pop operation, which removes an item from the stack. When an object is added to a stack, it is placed on the top of all previously entered items. When an item is removed, it can either be removed from the top or bottom of the stack. A stack in which items are removed the top is considered a "LIFO" (Last In, First Out) stack. 

Big O(n)

## Queues
A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO). A good example of a queue is any queue of consumers for a resource where the consumer that came first is served first. The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.
Queue is also an abstract data type or a linear data structure, just like stack data structure, in which the first element is inserted from one end called the REAR(also called tail), and the removal of existing element takes place from the other end called as FRONT(also called head).

Big O(n)

## Hash Tables

Hashing is a way of storing data that in an average case scenario allows for constant time storage and retrieval.
This can be achieved by using an array.

Hash Table Operations:

- Insert
- T [h(“john”)] = <“john”,25000>
- Delete
- T [h(“john”)] = NULL
- Search
- T [h(“john”)] returns the element hashed for “john”

Hash tables support fast insert and search:

- O(1) average case performance
- Deletion possible, but degrades performance
- Not suited if ordering of elements is important
- Many applications

## Sets 

## Binary Trees 
- A binary tree is a finite set of elements that are either empty or is partitioned into three disjointsubsets. The first subset contains a single element called the root of the tree. The other twosubsets are themselves binary trees called the left and right subtrees of the original tree. Aleft or right subtree can be empty. 
- Each element of a binary tree is called a node of the tree.
## Tries

## Balancing Binary Trees (AVL Tree)
