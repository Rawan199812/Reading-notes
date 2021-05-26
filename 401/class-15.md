## Trees

Node - A node is the individual item/data that makes up the data structure
Root - The root is the first/top Node in the tree
Left Child - The node that is positioned to the left of a root or node
Right Child - The node that is positioned to the right of a root or node
Edge - The edge in a tree is the link between a parent and child node
Leaf - A leaf is a node that does not contain any children


**Traversals**:An important aspect of trees is how to traverse them. 

- A tree allows us to search for a node, print out the contents of

- A tree, and much more! There are two categories of traversals

Trees:

- Depth First
- Breadth First

**Binary Trees**

***Binary Trees:restrict the number of children to two (hence our left and right children).There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows.***

***strategy for adding a new node to a binary tree is to fill all “child” spots from the top down. To do so, we would leverage the use of breadth first traversal. During the traversal, we find the first node that does not have 2 child nodes, and insert the new node as a child. We fill the child slots from left to right.***