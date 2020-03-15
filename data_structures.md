# Data Structures

## Arrays

Arrays are containers that allow access to its items through numerical indices,and it is single variable that is used to store different elements. It is often used when we want to store list of elements and access them by a single variable. Unlike most languages where array is a reference to the multiple variable,in JavaScript array is a single variable that stores multiple elements.

### Declaration of an Array
``` java

var House = [ ]; // method 1
var House = new array(); // method 2

```

### Initialization of an Array
``` java

var house = ["1BHK", "2BHK", "3BHK", "4BHK"];
```

or 
``` java

// Initializing while declaring 
// Creates an array having elements 10, 20, 30, 40, 50 
var house = new Array(10, 20, 30, 40, 50); 
  
//Creates an array of 5 undefined elements 
var house1 = new Array(5); 
  
//Creates an array with element 1BHK 
var home = new Array("!BHK"); 

```

### Accessing Array Elements

``` java

var house = ["1BHK", 25000, "2BHK", 50000, "Rent", true]; 
alert(house[0]+" cost= "+house[1]); 
var cost_1BHK = house[1]; 
var is_for_rent = house[5]; 
alert("Cost of 1BHK = "+ cost_1BHK); 
alert("Is house for rent = ")+ is_for_rent); 

```


### Length property of an Array

``` java

var house = ["1BHK", 25000, "2BHK", 50000, "Rent", true]; 
  
//len conatains the length of the array 
var len = house.length; 
for (var i = 0; i < len; i++) 
    alert(house[i]); 

```

### big O in array 

- Access - O(1)
- Appending - Amortized O(1) (sometimes resizing the hashtable is required; usually only insertion is required)
- Prepending - O(n) via unshift, since it requires reassigning all the indexes
- Insertion - Amortized O(1) if the value does not exist. O(n) if you want to shift existing values (Eg, using splice).
- Deletion - Amortized O(1) to remove a value, O(n) if you want to reassign indices via splice.
- Swapping - O(1)

## Linked List

## Stack 
A stack is a basic data structure that can be logically thought of as a linear structure represented by a real physical stack or pile, a structure where insertion and deletion of items takes place at one end called top of the stack. The basic concept can be illustrated by thinking of your data set as a stack of plates or books where you can only take the top item off the stack in order to remove things from it.

 This structure is used all throughout programming. The basic implementation of a stack is also called a LIFO (Last In First Out) to demonstrate the way it accesses data, since as we will see there are various variations of stack implementations. There are basically three operations that can be performed on stacks. They are 1) inserting an item into a stack (push). 2) deleting an item from the stack (pop). 3) displaying the contents of the stack (peek or top). 
 
 Applications of Stacks: 
 Converting a decimal number into a binary number. 
 Towers of Hanoi. 
 Expression evaluation and syntax parsing.
  An algorithm which has Quadratic Time Complexity.
  
   Big O Average Cases: insert,delete=(O(1)),search=(O(n)) . Worst Cases insert,delete=(O(1)),search=(O(n)) .

## Queues
Queue is an abstract data structure, which is open at both its ends.Queue follows First-In-First-Out methodology.
### Basic Operations:
* enqueue() − add (store) an item to the queue.
* dequeue() − remove (access) an item from the queue.
* peek() − Gets the element at the front of the queue without removing it.
* isfull() − Checks if the queue is full.
* isempty() − Checks if the queue is empty.
### Where to use:
you have to use Queues when things don't have to be processed immediately, but have to be processed in First In First Out order.
### Big-O:
#### Access: Θ(n)	
#### Search: Θ(n)	
#### Insertion: Θ(1)
#### Deletion: Θ(1)	

## Hash Tables 
* design A hash function is any function that can be used to map data of arbitrary size to fixed-size values. The values returned by a hash function are called hash values, hash codes, digests, or simply hashes. 
* operation using a parity-preserving operator like ADD or XOR.
*  big o is  O(1). 


## Sets 

## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)
