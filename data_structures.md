# Data Structures

## Arrays

## Linked List

## Stack 

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
