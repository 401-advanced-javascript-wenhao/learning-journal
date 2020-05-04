# Class15 - Career Coach & Tree Implementation - 5/1/2020

## Common Job Search Website
* Linkedin
* Glassdoor
* Monster
* Indeed
* Robert Half

## Tree Data Structure
* Tree
A tree is non-linear data structure, compared to arrays, linked lists, and stacks and queues which are linear data structures. A tree can be empty with no nodes or a tree is a structure consisting of a root node and zero or one or more subtrees.
* Example use of Tree Data Structure
HTML DOM Tree, Github branch structure
* Binary Tree
In a regular tree, a node can have any number of children. In a binary tree, a node can have at most two children - left child and right child. 
  * Breadth First Search (BFS)
  Traverse each node in the tree from lower level to higher level, from left to right.
  * Depth First Search (DFS)
  Starts at root node and traverse as far as possible along each branch before backtracking.
    * Preorder Traversal: Root -> Left -> Right
    * Inorder Traversal: Left -> Root -> Right
    * Postorder Traversal: Left -> Right -> Root
* Binary Search Tree
Binary Search Tree is a sorted binary tree, it has the following properties:
  * The left subtree of a node contains only nodes with value lesser than the node’s value.
  * The right subtree of a node contains only nodes with value greater than the node’s value.
  * The left and right subtree each must also be a binary search tree.