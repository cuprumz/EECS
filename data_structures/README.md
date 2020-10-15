### Data Structures

- [tree](https://en.wikipedia.org/wiki/Tree_(data_structure))
  - simulates a hierarchical tree structure, with root value and subtrees of children with a parent node, represented as a set of linked nodes.
- [binary tree](https://en.wikipedia.org/wiki/Binary_tree)
  - a tree data structure in which each node has at most two children, which are referred to as the left child and right child.
  - **full**(*proper* or *plane*) binary tree is a tree in which every node has either 0 or 2 children.
  - **complete** binary tree every level, except possibly the last, is completely filled, and all nodes in last level are as far left as possible. It can have between 1 and *2 to the h* nodes at the last level h.
  - **perfect** binary tree is a binary tree in which all interior nodes has two children and all leaves and all leaves have the same *depth* or same *level*
  - **balanced** binary tree is a binary tree structure in which the left and right subtrees of every node differ in height by no more than 1.
  - **infinite complete** binary tree
  - **degenerate**(*pathological*) tree, behave like a *linked list* data structure
  -  a perfect tree is therefore always complete but a complete tree is not necessarily perfect.
- [binary search tree](https://en.wikipedia.org/wiki/Binary_search_tree) BST
  - also called an **ordered** or **sorted binary tree**, is a [*rooted*](https://en.wikipedia.org/wiki/Rooted_tree) binary tree whose internal nodes each store a key greater than all the keys in the node's left subtree and less than whose in its right subtree.
- [B-tree](https://en.wikipedia.org/wiki/B-tree)
  - a self-balancing *tree data structure* that maintains sorted data and allows searches, sequential access, insertions, and deletions in logarithmic time.
  - generalizes the *binary search tree*, allowing for nodes with more than two children.
  - suited for storage systems that read and write relatively large blocks of data, such as disks.

- [B+ tree](https://en.wikipedia.org/wiki/B%2B_tree)
  - is an *m-ary tree* with a variable but often large number of children per node
  - can be viewed as a *B-tree* in which each node contains only keys (not key-value pairs), and to which and additional level is added at the bottom with linked leaves
  - the primary value of a B+ tree is in storing data for efficient retrieval in a block-oriented storage context, because very high fanout (number of pointers to child nodes in a node, typically on the order of 100 or more), which reduces the number of I/O operations required to find a element in the tree.

- [red-black tree](https://en.wikipedia.org/wiki/Red%E2%80%93black_tree)
  - a red-black tree is a kind of *self-balancing binary search tree*. Each node stores an extra bit representing color, used to ensure that the tree remains approximately balanced during insertions and deletions.