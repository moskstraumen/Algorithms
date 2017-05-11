# 树
##二叉树 (Binary Tree)
是每個節點最多有兩個子樹的樹結構。通常子樹被稱作「左子樹」（left subtree）和「右子樹」（right subtree）。

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

####Depth-first order
In depth-first order, we always attempt to visit the node farthest from the root node that we can, but with the caveat that it must be a child of a node we have already visited. Unlike a depth-first search on graphs, there is no need to remember all the nodes we have visited, because a tree cannot contain cycles. Pre-order is a special case of this. See depth-first search for more information.

####Breadth-first order[edit]
Contrasting with depth-first order is breadth-first order, which always attempts to visit the node closest to the root that it has not already visited. See breadth-first search for more information. Also called a level-order traversal.

In a complete binary tree, a node's breadth-index (i − (2d − 1)) can be used as traversal instructions from the root. Reading bitwise from left to right, starting at bit d − 1, where d is the node's distance from the root (d = ⌊log2(i+1)⌋) and the node in question is not the root itself (d > 0). When the breadth-index is masked at bit d − 1, the bit values 0 and 1 mean to step either left or right, respectively. The process continues by successively checking the next bit to the right until there are no more. The rightmost bit indicates the final traversal from the desired node's parent to the node itself. There is a time-space trade-off between iterating a complete binary tree this way versus each node having pointer/s to its sibling/s.

##二叉查找树(Binary Search Tree)
也称二叉搜索树、有序二叉树（英语：ordered binary tree），排序二叉树（英语：sorted binary tree），是指一棵空树或者具有下列性质的二叉树：
* 若任意节点的左子树不空，则左子树上所有结点的值均小于它的根结点的值；
* 若任意节点的右子树不空，则右子树上所有结点的值均大于它的根结点的值；
* 任意节点的左、右子树也分别为二叉查找树；
* 没有键值相等的节点。

二叉查找树相比于其他数据结构的优势在于查找、插入的时间复杂度较低。为O(log n)。

##平衡树
所有叶子的深度趋于平衡，更广义的是指在树上所有可能查找的均摊复杂度偏低。

##AVL树
AVL树是最先发明的自平衡二叉查找树。在AVL树中任何节点的节点的最大平衡因子为1
节点的平衡因子是它的左子树的高度减去它的右子树的高度（有時相反）。带有平衡因子1、0或 -1的节点被认为是平衡的。


##红黑树

红黑树是每个节点都带有颜色属性的二叉查找树，颜色为红色或黑色。在二叉查找树强制一般要求以外，对于任何有效的红黑树我们增加了如下的额外要求：
* 节点是红色或黑色。
* 根是黑色。
* 所有叶子都是黑色（叶子是NIL节点）。
* 每个红色节点必须有两个黑色的子节点。（从每个叶子到根的所有路径上不能有两个连续的红色节点。）
* 从任一节点到其每个叶子的所有简单路径都包含相同数目的黑色节点。


##B树
一般化的二元搜尋樹（binary search tree），可以拥有多于2个子节点。Each internal node of a B-tree will contain a number of keys. The keys act as separation values which divide its subtrees. Usually, the number of keys is chosen to vary between {\displaystyle d} d and {\displaystyle 2d} 2d, where {\displaystyle d} d is the minimum number of keys. The number of branches (or child nodes) from a node will be one more than the number of keys stored in the node. In a 2-3 B-tree, the internal nodes will store either one key (with two child nodes) or two keys (with three child nodes). A B-tree is sometimes described with the parameters {\displaystyle (d+1)} (d+1) — {\displaystyle (2d+1)} (2d+1) or simply with the highest branching order, {\displaystyle (2d+1)} (2d+1).


##2-3-4 树
在计算机科学中是阶为 4 的B树。
2-3-4 树把数据存储在叫做元素的单独单元中。它们组合成节点，每个节点都是下列之一
* 2-节点，就是说，它包含 1 个元素和 2 个儿子，
* 3-节点，就是说，它包含 2 个元素和 3 个儿子，
* 4-节点，就是说，它包含 3 个元素和 4 個儿子 。

##van Emde Boas树


##生成树