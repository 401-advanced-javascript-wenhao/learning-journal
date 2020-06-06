# Class 40 - CSS & Data Structures Recap - 6/5/2020 

## CSS  
* Display 
  * block - `<div>`, `<section>`, `<header>`, `<footer>`...
  * inline - `<img>`, `<a>`, `<span>`...
  * inline-block  
* Positioning 
  * relative
  * absolute  
  * fixed 
  * static  
  * inherit 

## Data Structures  
1. Linked List  
  * Description: sequence of nodes, starts with head node, ends with a null node, linear  
  * Node signature: value, next; next points to the next node in the list 
  * Strenghs: storage, traversal/insertion  
  * Weaknesses: traversal 
  * Time complexity - O(n)  
  * Space complexity - O(1) 
  * Use cases: pagination, block chain  

2. Stack  
  * Description: FILO (First In Last Out), stack of plates -> last plate added on the top of the plates is the first plate that you use 
  * Methods:  
    * peek: Looks at the top item in the stack  
    * pop: Removes the item from the top  
    * push: Adds the item to the top of the stack 
  * Strengths: FILO, push/pop, traversal  
  * Weaknesses: traversal 
  * Time complexity: O(n) 
  * Space complexity: O(1) -> push  
  * Use cases: call stack, undo/redo, history 

3. Queue  
  * Description: FIFO (First In First Out), standing in line -> first person in line is first into the movie  
  * Strengths: enqueque, dequeque 
  * Weaknesses: traversal 
  * Time complexity: O(n) 
  * Space complexity: O(1)  
  * Use cases: event queue, queue server  

4. Trees  
  * Description: Root node, each node has either children or no children
  * Binary Search Tree (BST) - sorted binary tree 
    * Strengths: time complexity - O(log(n)), insertion, deletion 
    * Traversal: Depth First Search (DFS), Breadth First Search (BFS) 
      * DFS:
        * pre-order: Data -> L -> R 
        * in-order: L -> Data -> R  
        * post-order: L -> R -> Data  
  * Binary Tree - could be sorted or not, node with no more that 2 children 
    * Traversal: DFS, BFS - O(n), aka level-order traversal 
  * Use cases: DOM Tree

5. Hash Map 
  * Description: key/value pair store; JS array with a defined size to "house" our data -> for each item we want to add to our store, we generate an index placement. That index placement also includes part of the key to handle collisions. We use LL for additional store 
  * Strengths: time complexity for lookup and insert is O(1)  
  * Weaknesses: Hashing algorithm, Linked List implementation for handling collisions -> possible O(n) traversal
  * Time complexity: O(1), possible O(n)  
  * Use cases: Dictionary 