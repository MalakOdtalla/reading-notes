# Reading Class 15

## Trees

A tree is non-linear and a hierarchical data structure consisting of a collection of nodes such that each node of the tree stores a value, a list of references to nodes (the “children”).

### Basic Terminology In Tree Data Structure:


Node - A Tree node is a component which may contain its own values, and references to other nodes

Root - The root is the node at the beginning of the tree

K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

Left - A reference to one child node, in a binary tree

Right - A reference to the other child node, in a binary tree

Edge - The edge in a tree is the link between a parent and child node

Leaf - A leaf is a node that does not have any children

Height - The height of a tree is the number of edges from the root to the furthest leaf

Sibling - Children of the same parent node are called siblings


### Types of Tree data structures

The different types of tree data structures are as follows:

1. General tree

A general tree data structure has no restriction on the number of nodes. It means that a parent node can have any number of child nodes.  

2. Binary tree  

A node of a binary tree can have maximum number of two child nodes. In the given tree diagram, node B, D, and F are left children, while E, C, and G are the right children.  

3. Balanced tree

If the height of the left sub-tree and the right sub-tree are equal or differs at most by 1, the tree is known as balanced tree data structure.  

4. Binary search tree

As the name implies, binary search trees are used for various searching and sorting algorithms.

## Why Tree? 
Unlike Array and Linked List, which are linear data structures, tree is hierarchical (or non-linear) data structure. 

One reason to use trees might be because you want to store information that naturally forms a hierarchy. For example, the file system on a computer: 
file system 

## Tree Traversals

Unlike linear data structures (Array, Linked List, Queues, Stacks, etc) which have only one logical way to traverse them, trees can be traversed in different ways. Following are the generally used ways for traversing trees.

- Depth First Traversals: 

(a) Inorder (Left, Root, Right) 

(b) Preorder (Root, Left, Right) 

(c) Postorder (Left, Right, Root) 

- Breadth-First or Level Order Traversal

for full understanding of Trees Traversals visit this [link](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)