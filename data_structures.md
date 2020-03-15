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