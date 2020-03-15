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

## Queues

## Hash Tables 

## Sets 

## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)
