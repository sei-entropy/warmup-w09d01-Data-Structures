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

## Queues

## Hash Tables 

## Sets 

## Binary Trees 

## Tries

## Balancing Binary Trees (AVL Tree)

AVL tree is a self-balancing Binary Search Tree (BST) where the difference between heights of left and right subtrees cannot be more than one for all nodes.

Most of the BST operations (e.g., search, max, min, insert, delete.. etc) take O(h) time where h is the height of the BST. The cost of these operations may become O(n) for a skewed Binary tree. If we make sure that height of the tree remains O(Logn) after every insertion and deletion, then we can guarantee an upper bound of O(Logn) for all these operations. The height of an AVL tree is always O(Logn) where n is the number of nodes in the tree.


### operations

* for insertion 

Step 1: First, insert a new element into the tree using BST's (Binary Search Tree) insertion logic.

Step 2: After inserting the elements you have to check the Balance Factor of each node.

Step 3: When the Balance Factor of every node will be found like 0 or 1 or -1 then the algorithm will proceed for the next operation.

Step 4: When the balance factor of any node comes other than the above three values then the tree is said to be imbalanced. Then perform the suitable Rotation to make it balanced and then the algorithm will proceed for the next operation. 


* for deletion

Step 1: Firstly, find that node where k is stored

Step 2: Secondly delete those contents of the node (Suppose the node is x)

Step 3: Claim: Deleting a node in an AVL tree can be reduced by deleting a leaf. There are three possible cases:

 When x has no children then, delete x
    When x has one child, let x' becomes the child of x.
    Notice: x' cannot have a child, since subtrees of T can differ in height by at most one :
        then replace the contents of x with the contents of x'
        then delete x' (a leaf)
 Step 4:  When x has two children,
        then find x's successor z (which has no left child)
        then replace x's contents with z's contents, and
        delete z

In all of the three cases, you will end up removing a leaf. 

### Big O 
* average
Θ(log(n))
 * worst
O(log(n))