# Data Structures

## Arrays
An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed,Each item in an array is called an element, and each element is accessed by its numerical index,Declaring a Variable to Refer to an Array
The preceding program declares an array (named anArray)
anArray = new int[10];
The next few lines assign values to each element of the array:
anArray[0] = 100; // initialize first element
anArray[1] = 200; // initialize second element
anArray[2] = 300; // and so forth
Each array element is accessed by its numerical index:
System.out.println(“Element 1 at index 0: ” + anArray[0]);
System.out.println(“Element 2 at index 1: ” + anArray[1]);
System.out.println(“Element 3 at index 2: ” + anArray[2]);
Alternatively, you can use the shortcut syntax to create and initialize an array:
int[] anArray = {
    100, 200, 300,
    400, 500, 600,
    700, 800, 900, 1000
};
 following MultiDimArrayDemo program:
class MultiDimArrayDemo {
    public static void main(String[] args) {
        String[][] names = {
            {“Mr. “, “Mrs. “, “Ms. “},
            {“Smith”, “Jones”}
        };
        // Mr. Smith
        System.out.println(names[0][0] + names[1][0]);
        // Ms. Jones
        System.out.println(names[0][2] + names[1][1]);
    }
}
Finally, you can use the built-in length property to determine the size of any array. The following code prints the array’s size to standard output:
 System.out.println(anArray.length);
 Big O array in search o(n)

## Linked List
The simplest form of linked lists — a singly linked list — is a series of nodes where each individual node contains both a value and a pointer to the next node in the list.
Additions (Add) grow the list by adding items to the end of the list.
Removals (Remove) will always remove from a given position in the list.
Search (Contains) will search the list for a value.
Each element (we will call it a node) of a list is comprising of two items - the data and a reference to the next node. The last node has a reference to null. The entry point into a linked list is called the head of the list. It should be noted that head is not a separate node, but the reference to the first node. If the list is empty then the head is a null reference.
A linked list is a dynamic data structure. The number of nodes in a list is not fixed and can grow and shrink on demand. Any application which has to deal with an unknown number of objects will need to use a linked list.
One disadvantage of a linked list against an array is that it does not allow direct access to the individual elements. If you want to access a particular item then you have to start at the head and follow the references until you get to that item.
Another disadvantage is that a linked list uses more memory compare with an array - we extra 4 bytes (on 32-bit CPU) to store a reference to the next node.
Types of Linked Lists
A singly linked list is described above
A doubly linked list is a list that has two references, one to the next node and another to previous node.
 Big O singly linked list in search o(n)
 Big O doubly linked list in search o(n)

## Stack 
Operate on “last-in, first-out”(LIFO)behavior. The last, most recently added item, is the first to be removed.
#### Example: 
 “back” button on your browser.
 #### Big O
| Function  | Complexity|
| ------------- | ------------- |
| Access | O(1) |
| Insert | O(1)  |
| Delete  | O(1)  |
| Check empty | O(1) |

=======
## Queues
Operate on “first-in, first-out”(FIFO) behavior. Items are removed in the order they were added, from first to last.
#### Example: 
The ordeer of print document using FIFO.
#### Big O:
| Function  | Complexity|
| ------------- | ------------- |
| Access | O(1) |
| Insert | O(1)  |
| Delete  | O(1)  |
| Check empty | O(1) |

## Hash Tables 

- Is used to uniquely identify a specific object - From a group of similar objects.
(for Example: In libraries, each book is assigned a unique number that can be used to determine information about the book, so books were hashed to a unique number ) 
- large keys are converted into small keys by using hash functions, The values are then stored in a data structure called hash table.
- Using Array to distribute entries (key/value pairs) uniformly.

 Big O :
- Each element is assigned a key (converted key). By using that key you can access the element in O(1) time.

## Sets 

- is an abstract data type that can store unique values, without any particular order.
- can be implemented using various data structures, which provide different time and space trade-offs for various operations.

 Big O :
- for sorted sets (which has O(log n) for most operations).

## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)
