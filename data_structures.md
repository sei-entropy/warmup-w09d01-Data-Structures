# Data Structures

## Arrays

## Linked List
linked list consists of nodes where each node contains a data field and a reference(link) to the next node in the list.

Types of Linked Lists:
A singly linked list: contain nodes which have a data field as well as 'next' field, which points to the next node in line of nodes. Operations that can be performed on singly linked lists include insertion, deletion and traversal.
A doubly linked list: is a list that has two references, one to the next node and another to previous node.

Time complexities:
Indexing	Θ(n)
Insert/delete at beginning	Θ(1)
Insert/delete at end	Θ(1) when last element is known;
Θ(n) when last element is unknown
Insert/delete in middle	search time + Θ(1)
Wasted space (average)	Θ(n)

## Stack 
A stack is a basic data structure that can be logically thought of as a linear structure represented by a real physical stack or pile, a structure where insertion and deletion of items takes place at one end called top of the stack

What type of data structure is a stack?

Stack is an ordered list of similar data type. Stack is a LIFO(Last in First out) structure 
or we can say FILO(First in Last out). 

Stack set of operations:

push - add a new item on top of the stack
pop - remove the top item from the stack
isEmpty - check if the stack is empty
size - count the number of items on the stack

Time complexities:
Push Operation : O(1)
Pop Operation : O(1)
Top Operation : O(1)
Search Operation : O(n)

Position of Top               Status of Stack
                               
     -1	                       Stack is Empty
      0	                    Only one element in Stack
     N-1	                        Stack is Full
      N	                  Overflow state of Stack

## Queues

## Hash Tables 
  Hash Tables:Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects.

Hashing is implemented in two steps:

An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
The element is stored in the hash table where it can be quickly retrieved using hashed key.

hash = hashfunc(key)
index = hash % array_size

Hash function
A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.

In terms of manipulating dataset, such as lookup, insertion, deletion, and search, Hash tables have huge advantage since it has key — value based structure. If every element is where it should be the the search can use a single comparison to discover the presence of an element. It means that searching for the element takes same amount of time as searching for the first element of an array, which is a constant time or O(1). However, if our dataset is bigger than hash table collisions occur and we need to deal with them using different methods. It takes also constant time to insert and delete an element because the hash function determines where to save or remove it.

## Sets 

A set is a data structure that can store any number of unique values in any order you so wish. Set’s are different from arrays in the sense that they only allow non-repeated, unique values within them.


## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)

Binary search trees provide O(log N) search times provided that the nodes are distributed in a reasonably “balanced” manner. Unfortunately, that is not always the case and performing a sequence of deletions and insertions can often exacerbate the problem.
When a BST becomes badly unbalanced, the search behavior can degenerate to that of a sorted linked list, O(N).
There are a number of strategies for dealing with this problem; most involve adding some sort of restructuring to the insert/delete algorithms.
That can be effective only if the restructuring reduces the average depth of a node from the root of the BST, and if the cost of the restructuring is, on average, O(log N).

Algorithm		Average  	Worst case
Space		     O(n)O(n)	O(n)O(n)
Search	O(logn)O(\log n)    O(log⁡n)O(\log n)
Insert	O(logn)O(\log n)	O(logn)O(\log n)
Delete	O(logn)O(\log n)	O(logn)O(\log n)
