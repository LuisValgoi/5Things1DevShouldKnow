# 💡 Summary
- [General Concepts](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#what-is-abstract-data-types)
- [Data Structures Examples](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#data-structure-examples)
    - [Array](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#array)
    - [Linked Lists](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#linked-lists)
    - [Doubly Linked Lists](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#doubly-linked-lists)
    - [Stack](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#stack)
    - [Queue](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#queue)
    - [BST - Binary Search Trees](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#bst---binary-search-trees)
    - [AVL](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#avl)
    - [Red Black Tree](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#red-black-tree)
    - [Splay Tree](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#splay-tree)
    - [B-Trees](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#b-trees)
    - [2-3 B-Trees](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#2-3-b-trees)
    - [Priority Queues](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#priority-queues)
    - [Heap](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#heap)
    - [Heap Sort](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#heap-sort)
    - [HashTables / Dictionaries](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#hashtables--dictionaries)
---
---
---
# What is Abstract Data Types?
* It is the interface.
* Model for a certain data structure. 
* Like supertype in programming.
* Ex: Stack / Queue.

# What is Data Structures?
* It is the concrete implementation.
* Able to CRUD data in a efficient way.
* Ex: Arrays / Linked Lists / Binary Trees.

# Data Structure Examples

## Array
* It is a DS.
* Static Type Structure.
* Easily to find if you know the position.
* Very fast data structure.
* **Operations:**
    * Find: O(1)
    * Add / Remove Last: O(1)
    * Remove Position: O(n)

## Linked Lists
* It is a DS.
* Dynamic Structure.
* Allocated memory in run-time.
* To navigate backwards is extremally difficult (Doubly Linked List is very good).
* Has a pointers to the next node.
* **Operations:**
    * Find: O(n)
    * Add / Remove Beggining: O(1)
    * Add / Remove Position: O(n)

## Doubly Linked Lists
* It is a DS.
* Not so memory friendly.
* Can be traversed in both directions.
* Set of nodes that points one to another (previous node and next node).
* **Operations:**
    * Remove Position: O(n)

## Stack
* It is a ADT.
* Basic operations: pop(), peek(), push().
* LIFO Structure.
* Most important app: Stack Memory
* **Operations:**
    * Push / Pop / Peek: O(1)

## Queue
* It is a ADT.
* Basic Operations: enqueue(), dequeue().
* FIFO Structure.
* Most important app: CPU Scheduling.
* **Operations:**
    * Enqueue / Dequeue : O(1)

## BST - Binary Search Trees
* It is DS.
* Basic idea to reduce O(N) search to O(logN).
* Is a binary search tree when each node have 2 distinguished sub-trees.
* Might be Unbalanced.
* Keeps the elements sorted.
* Much better than linear comparison, since the path is splited in the half proportionally.
* **Operations:**
    * Find: O(logN)
    * Any Operation: O(logN)

## AVL
* It is the solution for BST (unbalanced trees).
* It is a balanced tree.
* We use them when we need to search a lot (because is rigidly balanced).
* The heigth of two child subtrees of any node differ by at most one.
    * For that level, its root node can differ at most +1 or -1
* AVL > ReedBlackTrees.
* The only different operations is during the insertion.
    * You must check if after the insertion, the binary tree is balanced.
* **Most Used Apps:**
    * Operational Systems

## Red Black Tree
* Each node is red or black.
* The root node is always black.
* Every red node must have 2 black child node.
* Every leaf is point to a NIL/NULL.
* Every path from a give node contains to any of its descendent contains the same number of black nodes.
* We use them when we need to insert/remove a lot (because is not rigidly balanced).

## Splay Tree
* It is a type of a BST.
* Most O(logN) but some O(n)
* It is not Strictly Balanced Data Structure.
* Basically, the only difference is that when we fined the give node, we turn it into the root node (it is called SPLAYING).
    * That happens because when we want to find it again, it is going to be O(1).
* **Most Used Apps:**
    * Cache

## B-Trees
* Self balanced trees like Data Structures.
* Nodes might have more than 2 child.
* Each node contains multiple keys.
* It does not need balancing (but might waste some space).
* Optmized for systems that Read and Write large blocks of the data.
* **Most Used Apps:**
    * External Memory
* **Operations:**
    * CRUD: O(logN)

## 2-3 B-Trees
* Every node can have 2 data elements at most.
* Every node can have 3 children at most.
* All leafs are on the same level.
* All data is kept in sorted order.

## Priority Queues
* It is an ADT.
* Every single value has a additional prop: Priority Value.
* The priority number indicates which "node" is going to be the next.
* In a Priority Queue, the high priority value (highest) comes first then the lower priority value (lowest).
* It is usually implemented with Heap.
* Very similar to the Queue.
* DESC (Max to Lowest).

## Heap
* It is a DS.
* It is like a binary tree.
* It is line by line. 
* Its flow is always from LEFT to RIGHT.
* It does not matter the smallest / highest read.
* The only rule is that the parent must contains the MAX / MIN value.
* Its completion works like that: ROOT, LEFT, RIGHT (Root > Left > Right > left of the L , right of the L, left of the R, right of the R).
* We assign index to HEAP and we read it in a dimensional array.
* Root: "i" / Left Node: "2 * i + 1" / Right node: "2 * i + 2".
* **Operations:**
    * Reconstruct: O(logN)
    * Insert: O(logN)
    * Deletion: O(logN)
    * Find MAX/MIN: O(1)

## Heap Sort
* It is a sort algorithm (like QuickSort).
* Uses HeapSort to find the MAX value.
* It has a best worst case runtime.
* If we find the item, we set it to visit (do not look for it again).
* It is not a stable sort.
* **Operations:**
    * Sorting: O(N * logN)

## HashTables / Dictionaries
* Collection of key-value pair.
* "Collisions" is when we have multiple keys for the same bucket
    * We must use "Chaining": Indexes as Linked List for multiples indexes.
    * We must use "Linear Probing": Find the next empty slot in the array.
* Perfomance depends on the Load Factor.
    * Load Factor: number of entries / number of buckets.
    * Dynamic Resizing is need sometimes.
* **Operations:**
    * Insertion: 0(1) 
    * Search: 0(1) 
