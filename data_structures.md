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

## Sets 

## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)
