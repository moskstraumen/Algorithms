# 树
##二叉树
是每個節點最多有兩個子樹的樹結構。通常子樹被稱作「左子樹」（left subtree）和「右子樹」（right subtree）。
####二元樹
二元树是一個有根树，並且每個節點最多有2個子節點.
####Full binary tree 
Sometimes referred to as a proper or plane binary tree is a tree in which every node in the tree has either 0 or 2 children.




####Perfect binary tree 
Binary tree in which all interior nodes have two children and all leaves have the same depth or same level.[18] (This is ambiguously also called a complete binary tree.[19]) An example of a perfect binary tree is the ancestry chart of a person to a given depth, as each person has exactly two biological parents (one mother and one father).

####Complete binary tree 
Every level, except possibly the last, is completely filled, and all nodes in the last level are as far left as possible. It can have between 1 and 2h nodes at the last level h. An alternative definition is a perfect tree whose rightmost leaves (perhaps all) have been removed. Some authors use the term complete to refer instead to a perfect binary tree as defined above, in which case they call this type of tree an almost complete binary tree or nearly complete binary tree. A complete binary tree can be efficiently represented using an array.

####Pre-order

* Check if the current node is empty / null.
* Display the data part of the root (or current node).
* Traverse the left subtree by recursively calling the pre-order function.
* Traverse the right subtree by recursively calling the pre-order function.

####In-order

* Check if the current node is empty / null.
* Traverse the left subtree by recursively calling the in-order function.
* Display the data part of the root (or current node).
* Traverse the right subtree by recursively calling the in-order function.
* In a search tree, in-order traversal retrieves data in sorted order.[4]

####Post-order

* Check if the current node is empty / null.
* Traverse the left subtree by recursively calling the post-order function.
* Traverse the right subtree by recursively calling the post-order function.
* Display the data part of the root (or current node).

#### Depth-first order
In depth-first order, we always attempt to visit the node farthest from the root node that we can, but with the caveat that it must be a child of a node we have already visited. Unlike a depth-first search on graphs, there is no need to remember all the nodes we have visited, because a tree cannot contain cycles. Pre-order is a special case of this. See depth-first search for more information.

Breadth-first order[edit]
Contrasting with depth-first order is breadth-first order, which always attempts to visit the node closest to the root that it has not already visited. See breadth-first search for more information. Also called a level-order traversal.

In a complete binary tree, a node's breadth-index (i − (2d − 1)) can be used as traversal instructions from the root. Reading bitwise from left to right, starting at bit d − 1, where d is the node's distance from the root (d = ⌊log2(i+1)⌋) and the node in question is not the root itself (d > 0). When the breadth-index is masked at bit d − 1, the bit values 0 and 1 mean to step either left or right, respectively. The process continues by successively checking the next bit to the right until there are no more. The rightmost bit indicates the final traversal from the desired node's parent to the node itself. There is a time-space trade-off between iterating a complete binary tree this way versus each node having pointer/s to its sibling/s.
##红黑树


##van Emde Boas树


##生成树