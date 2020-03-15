# Data Structures

## Arrays

## Linked List

## Stack 
A stack is a basic data structure that can be logically thought of as a linear structure represented by a real physical stack or pile, a structure where insertion and deletion of items takes place at one end called top of the stack. 
The basic implementation of a stack is also called a `LIFO` (Last In First Out) .

#####  Operations of stack :
* `push(new-item:item-type)`
Adds an item onto the stack.
* `top():item-type`
Returns the last item pushed onto the stack.
* `pop()`
Removes the most-recently-pushed item from the stack.
* `is-empty():Boolean`
True if no more items can be popped and there is no top item.
* `is-full():Boolean`
True if no more items can be pushed.
* `get-size():Integer`
Returns the number of elements on the stack.
* All operations except `get-size()` can be performed in `O(1)` time. 
`get-size()` runs in at worst `O(N)`.


![](https://schwarztiger.files.wordpress.com/2018/08/stack_representation.jpg?w=500)

## Queues
Queue is a linear data structure where the first element is inserted from one end called REAR and deleted from the other end called as FRONT.
Queue follows the `FIFO` (First - In - First Out) structure.

##### Operations of queues : 
* `enqueue()` 
Adding an element into queue.
* `dequeue()`
Removing an element from queue.
* `init()`
Used for initializing the queue.
* `Front` 
Front is used to get the front data item from a queue.
* `Rear` 
Rear is used to get the last item from a queue. 
##### Queue Implementation :
`Array` is the easiest way to implement a queue. Queue can be also implemented using Linked List or Stack.
![](https://www.tutorialride.com/images/data-structures/queue-array.jpeg)


## Hash Tables 

## Sets 

## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)
