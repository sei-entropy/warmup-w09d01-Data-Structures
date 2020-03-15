# Data Structures

## Arrays
##### Design And Operations:
###### Design
Arrays in javascript are objects which contain a list of items. They are considered as ordered collection of values where each value is called an element and each element has a numeric position in the array, known as index.

An element inside an array can be of any type, and different elements of the same array can be of different types: string, boolean, number, objects or even other arrays.

###### Some Operations in JS
Create an Array
``` js
let fruits = ['Apple', 'Banana']
console.log(fruits.length)
// 2
```

Access (index into) an Array item
``` js
let first = fruits[0]
// Apple
let last = fruits[fruits.length - 1]
// Banana
```

Loop over an Array
```js
fruits.forEach(function(item, index, array) {
  console.log(item, index)
})
// Apple 0
// Banana 1
```

Add to the end of an Array
```js
let newLength = fruits.push('Orange')
// ["Apple", "Banana", "Orange"]
```

Remove from the end of an Array
```js
let last = fruits.pop() // remove Orange (from the end)
// ["Apple", "Banana"]
```

Remove from the front of an Array
```js
let first = fruits.shift() // remove Apple from the front
// ["Banana"]
```

Add to the front of an Array
```js
let newLength = fruits.unshift('Strawberry') // add to the front
// ["Strawberry", "Banana"]
```

Find the index of an item in the Array
```js
fruits.push('Mango')
// ["Strawberry", "Banana", "Mango"]

let pos = fruits.indexOf('Banana')
// 1
```

Remove an item by index position
```js
let removedItem = fruits.splice(pos, 1) // this is how to remove an item
                                        
// ["Strawberry", "Mango"]
```

Remove items from an index position
```js
let vegetables = ['Cabbage', 'Turnip', 'Radish', 'Carrot']
console.log(vegetables)
// ["Cabbage", "Turnip", "Radish", "Carrot"]

let pos = 1
let n = 2

let removedItems = vegetables.splice(pos, n)
// this is how to remove items, n defines the number of items to be removed,
// starting at the index position specified by pos and progressing toward the end of array.

console.log(vegetables)
// ["Cabbage", "Carrot"] (the original array is changed)

console.log(removedItems)
// ["Turnip", "Radish"]
```

Copy an Array
```js
let shallowCopy = fruits.slice() // this is how to make a copy
// ["Strawberry", "Mango"]
```

##### General Use:
It is often used when we want to store list of elements and access them by a single variable. Unlike most languages where array is a reference to the multiple variable, in JavaScript array is a single variable that stores multiple elements.

##### BigO:
* Access - O(1)
* Appending - Amortized O(1) (sometimes resizing the hashtable is required; usually only insertion is required)
* Prepending - O(n) via unshift, since it requires reassigning all the indexes
* Insertion - Amortized O(1) if the value does not exist. O(n) if you want to shift existing values (Eg, using splice).
* Deletion - Amortized O(1) to remove a value, O(n) if you want to reassign indices via splice.
* Swapping - O(1)

## Linked List
##### Design and Operations
A linked list is a data structure that stores multiple values in a linear fashion. Each value in a linked list is contained in its own node, an object that contains the data along with a link to the next node in the list. The link is a pointer to another node object or null if there is no next node. If each node has just one pointer to another node (most frequently called next) then the list is considered a singly linked list (or just linked list) whereas if each node has two links (usually previous and next) then it is considered a doubly linked list.

##### General Use:
Linked lists are often used because of their efficient insertion and deletion. They can be used to implement stacks, queues, and other abstract data types.

##### BigO:
* Indexing O(n)
* Insert/delete at beginning O(1)
* Insert/delete at end O(1)
* Insert/delete in middle O(1)+O(n)

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




## References
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array
* https://hackernoon.com/work-with-javascript-arrays-like-a-boss-97207a042e42
* https://stackoverflow.com/questions/11514308/big-o-of-javascript-arrays
* https://humanwhocodes.com/blog/2019/01/computer-science-in-javascript-linked-list/
* https://brilliant.org/wiki/linked-lists/
* https://stackoverflow.com/questions/22134540/what-are-the-relevant-big-o-notations-for-linked-lists