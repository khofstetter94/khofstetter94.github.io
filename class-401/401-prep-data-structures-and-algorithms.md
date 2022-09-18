# Data Structures and Algorithms

[Basic Recurions](https://www.youtube.com/watch?v=vPEJSJMg4jY)

- Recursion is when a function calls itself
- Recursion is used when it makes the solution clearer
- Every recursive function has two parts: the base case (when the function doesn't call itself) and the recursive case (when the function calls itself)

[Data Structures in 15 Minutes](https://www.youtube.com/watch?v=sVxBVvlnJsM)

- Compound data is data items grouped together
- Big O Notation: measuring how well a data structure does a specific thing, how well an operation scales
- Linked lists
  - the atomic unit of a linked list is called a "node" which contains a value and a pointer, with each pointer pointing to the next node
  - the first node is known as the head while the last one is known as the tail
  - Great at adding and deleting nodes, but bad at retrieving nodes even when we know the index (each node is only aware of the node next to it)
- Array
  - A continuous block of cells in the computer memory
  - Really good at retrieving items, but bad at adding items because we may need to move the array to a new place so that it fits
- Hash Table
  - An object in JavaScript
  - Key value pairs, like a dictionary providing a term and a definition
  - The key goes into a "hashing function" and it will spit out a memory location for you, these memory locations do not need to be next to eachother, they can be anywhere
  - Two keys can hash to the same memory location, known as a "collision"
  - Great at retrieving and adding, but bad because of collisions
- Stack and queue
  - Stack is a "last in, first out" data structure
  - Using .push() and .pop()
  - Every language keeps track of the functions that have been called by using the call stack
  - Stacks are important for an algoithm called DFS (depth-first search)
  - Queue is "first in, first out", like standing in line for something
  - Adding an item uses .enqueue(),  removing from the front is .dequeue()
  - Queues are used for an algorithm called breadth-first search
  - Stacks and queues are efficient in adding and removing but have limited use cases
- Graphs and Trees
  - Graphs are similar to linked lists but the pointers are called edges and they can have weights or numbers assigned to them
  - With trees, the data expands out in one direction, kinda like a family tree or HTML tree with nested elements
  - A Binary search tree has rules but it makes searching really efficient - each node can only have a max of two children (left and right), the left as to be less than the parent node and the right has to be more
  - Can be unbalanced and you can lost the advantages you get with your search optimization

[Big O Explained](https://www.youtube.com/watch?v=v4cd1O4zkGw)

- Big O also known as algorithmic efficiency - how time scales with respect to some input variables
- Transfer speed is O(1), its constant time with respect to the size of the input. It doesnt take longer with more input
- The internet transfer time is O(n), it scales linearly with respect to the amount of input
- Rules for Big O:
  - If you have two different steps in your algoithm, you add up those steps
  - Drop constants
  - If you have different inputs, you're usually going to use different variables to represent them
  - Drop non-dominant terms

[Basic Data Structures](https://towardsdatascience.com/8-common-data-structures-every-programmer-must-know-171acf6a1a42)

- Data Structures are a specialized means of organizing and storing data in computers in such a way that we can perform operations on the stored data more efficiently
- Arrays
  - a structure of fixed-size, which can hold items of the same data type. They are indexed
  - Array operations
    - Traverse: Go through the elements and print them.
    - Search: Search for an element in the array. You can search the element by its value or its index
    - Update: Update the value of an existing element at a given index
  - Inserting elements to an array and deleting elements from an array cannot be done straight away as arrays are fixed in size
  - Applications of arrays
    - Used as the building blocks to build other data structures such as array lists, heaps, hash tables, vectors and matrices.
    - Used for different sorting algorithms such as insertion sort, quick sort, bubble sort and merge sort.
- Linked Lists
  - a sequential structure that consists of a sequence of items in linear order which are linked to each other.
  - access data sequentially and random access is not possible. Provides a simple and flexible representation of dynamic sets
  - Elements in a linked list are known as nodes.
  - Each node contains a key and a pointer to its successor node, known as next.
  - The attribute named head points to the first element of the linked list.
  - The last element of the linked list is known as the tail
  - Linked list types:
    - Singly linked list — Traversal of items can be done in the forward direction only.
    - Doubly linked list — Traversal of items can be done in both forward and backward directions. Nodes consist of an additional pointer known as prev, pointing to the previous node.
    - Circular linked lists — Linked lists where the prev pointer of the head points to the tail and the next pointer of the tail points to the head.
  - Linked list operations
    - Search: Find the first element with the key k in the given linked list by a simple linear search and returns a pointer to this element
    - Insert: Insert a key to the linked list. An insertion can be done in 3 different ways; insert at the beginning of the list, insert at the end of the list and insert in the middle of the list.
    - Delete: Removes an element x from a given linked list. You cannot delete a node by a single step. A deletion can be done in 3 different ways; delete from the beginning of the list, delete from the end of the list and delete from the middle of the list.
- Stacks
  - a LIFO (Last In First Out — the element placed at last can be accessed at first) structure. This structure is named as “stack” because it resembles a real-world stack — a stack of plates
  - Stack operations
    - Push: Insert an element on to the top of the stack
    - Pop: Delete the topmost element and return it
    - Peek: Return the top element of the stack without deleting it
    - isEmpty: Check if the stack is empty
    - isFull: Check if the stack is full
  - Applications of stacks
    - Used for expression evaluation (e.g.: shunting-yard algorithm for parsing and evaluating mathematical expressions)
    - Used to implement function calls in recursion programming
- Queues
  - a FIFO (First In First Out — the element placed at first can be accessed at first) structure. This structure is named as “queue” because it resembles a real-world queue — people waiting in a queue
  - Queue operations
    - Enqueue: Insert an element to the end of the queue
    - Dequeue: Delete the element from the beginning of the queue
  - Applications of queues
    - Used to manage threads in multithreading
    - Used to implement queuing systems (e.g.: priority queues)
- Hash Tables
  - a data structure that stores values which have keys associated with each of them, supports lookup efficiently if we know the key associated with the value, efficient in inserting and searching, irrespective of the size of the data
  - Direct Addressing uses the one-to-one mapping between the values and keys when storing in a table. But when there is a large number of key-value pairs, the table will be huge with so many records and may be impractical or even impossible to be stored, given the memory available on a typical computer
  - Hash Function: A special function named as the hash function (h) is used to overcome the aforementioned problem in direct addressing
  - We can resolve collisions by selecting a suitable hash function h and use techniques such as chaining and open addressing
- Trees
  - a hierarchical structure where data is organized hierarchically and are linked together
  - A binary search tree (BST), as the name suggests, is a binary tree where data is organized in a hierarchical structure. This data structure stores values in sorted order.
    - Attributes in a binary search tree:
      - key: The value stored in the node
      - left: The pointer to the left child
      - right: The pointer to the right child
      - p: The pointer to the parent node
  - Applications of trees:
    - Binary Trees: Used to implement expression parsers and expression solvers
    - Binary Search Tree: used in many search applications where data are constantly entering and leaving
    - Heaps: used by JVM (Java Virtual Machine) to store Java objects
    - Treaps: used in wireless networking
- Heaps
  - a special case of a binary tree where the parent nodes are compared to their children with their values and are arranged accordingly
  - Heaps can be of 2 types:
    - Min Heap — the key of the parent is less than or equal to those of its children. This is called the min-heap property. The root will contain the minimum value of the heap.
    - Max Heap — the key of the parent is greater than or equal to those of its children. This is called the max-heap property. The root will contain the maximum value of the heap.
- Graphs
  - A graph consists of a finite set of vertices or nodes and a set of edges connecting these vertices
  - The order of a graph is the number of vertices in the graph
  - The size of a graph is the number of edges in the graph
  - Two nodes are said to be adjacent if they are connected to each other by the same edge
  - Directed Graphs: if all its edges have a direction indicating what is the start vertex and what is the end vertex
    - We say that (u, v) is incident from or leaves vertex u and is incident to or enters vertex v
    - Self-loops: Edges from a vertex to itself
  - Undirected Graphs: all its edges have no direction. It can go in both ways between the two vertices.
    - If a vertex is not connected to any other node in the graph, it is said to be isolated

[Why Big O](https://triplebyte.com/blog/why-you-should-learn-big-o-and-stop-hacking-your-way-through-algorithms)

- Big-O is just a notation used to describe how efficient an algorithm is
- “the time complexity of this function is O(n).” The letter “O” can just be thought of as shorthand for the rough “order” of magnitude of operations it takes to run the function, while “n” represents the possible number of vegetables passed in each time
- Efficiency is the entire point
  - The entire reason algorithms exist is to make our lives easier. They allow our code to run in a reasonable amount of time and take up a reasonable amount of space
- Missing the point makes learning harder
  - If you think about algorithms without reference to time and space (as arbitrary sets of instructions), they lose their meaning. If you think about them together, as two critical parts of the same narrative, everything becomes interesting
- Getting the point also prevents mistakes
  - And on top of making learning easier, understanding the point of Big-O (and algorithms in general) will seriously help you avoid mistakes in interviews

## Discussion Questions

- What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?
  - The size of the data and the size of the storage. The problem that needs to be solved and the operations needed to solve it.
- How can we ensure that we’ll avoid an infinite recursive call stack?
  - Utilizing the base case of the recursive function which doesn't call the function itself again

### Things I want to know more about

- All of this, this was a ton of information. I want to understand each data structure thoroughly and discuss the Big O in more depth. I think this topic will need a lot of study and practice on my end.

[Return home](https://khofstetter94.github.io/reading-notes/)
