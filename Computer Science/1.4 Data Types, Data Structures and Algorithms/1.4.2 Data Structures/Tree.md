# Tree
2022-12-09 | [1.4.2 Data Structures](1.4.2%20Data%20Structures.md)

- **Tree** -> An undirected graph with no cycles
	- There is only one possible path between two nodes
- **Root** -> Start node of the tree for traversals
	- **Rooted tree** -> Tree with a root
- **Parent** -> The node that is above a node in the hierarchy
- **Child** -> The node that is below a node
- **Siblings** -> Multiple nodes that come from the same parent
- For any tree: $\text{No. of Edges} = \text{No. of Nodes} - 1$
- **Leaf** -> End-point on a tree, a point that isn't a parent (has no children)
- **Branch** -> A path from the root to a leaf
- **Height** -> The length of the largest branch
- **Sub-tree** -> A tree inside of a tree

## Binary Tree
- **Binary Tree** -> A rooted tree where every node has at most two child nodes
- **Binary Search Tree** -> Binary tree where nodes are also ordered
	- If the order is ascending (low to high), the nodes of the left sub-tree have values that are lower than the root, and the nodes of the right sub-tree have values that are higher than the root
- The tree cannot be binary if it isn't rooted
![A binary search tree](https://isaaccomputerscience.org/api/v3.3.1/api/images/content/computer_science/data_structures_and_algorithms/data_structures/figures/isaac_cs_dsa_data_struct_lettered_tree.png)

## Expression Tree
- **Binary Expression Tree** -> Used to represent an expression such as algebraic or boolean
	- Leaf nodes contain operands and other nodes contain operators
![A mathematical expression tree](https://isaaccomputerscience.org/api/v3.3.1/api/images/content/computer_science/data_structures_and_algorithms/data_structures/figures/isaac_cs_dsa_data_struct_expression_tree.png)

## Uses
- Binary trees are used in compilers to build syntax trees, and are used within routers to store routing tables
- Binary search trees can be built to speed up searching
- Expression trees can be used to represent algebraic and Boolean expressions in a way that simplifies the processing of the expression
