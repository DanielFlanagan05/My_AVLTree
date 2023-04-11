# My_AVLTree
An AVL Tree I implemented for my algorithms and data structures class.

Nodes in this implementation hold the necessary pointers which point to its parent, left and right nodes. It also holds the value of the Node and the height of the Node. Nodes also have a data pointer which allows them to store additional information relevant to the application problem of this assignment, which was the Table class implementation (see third paragraph).

This AVL Tree implementataion includes member functions to return Python generators that represent the tree in inorder, preorder, postorder and levelorder traversals. Other member functions provide utility such as returning the maximum or minimum Nodes, and handling insertions which prompt the tree to rebalance itself using right and/or left rotations when necessary. There is also a search member function to find and return a node with a specified value.
Removal and visualization functionality was provided by my professor within the project's template.

I also implemented a Table class with functions to test use cases relevant to a database. This class utilizes the data pointer within the Node class, which I use to store a list of strings. Member functions include insert_rows(), which takes a list of lists of strings containing values, and a list of strings containing the values' corresponding attributes. The function instantiates nodes within the AVL tree using the insert() function, and reorders rows (inner lists) from values to properly correspond with the attribute the value represents. The row is inserted to the Node's data pointer, and their value is their insertion index, which is correspondant to the order by which the row is inserted. This class also contains functions to remove specified rows by their index, show the latest row (which is the row with the highest insertion index, and therefore value), show the oldest row, and show all of the data stored within the tree.

Note only the "solution.py" file is my own work, and work within it that is not mine is specified. 
To be specific though:
Within the AVL_Tree class right_rotate, balance_factor, rebalance, insert, min, max, search, inorder, __iter__, preorder, postorder, and levelorder is my own work.
Within the Table class all functions except for the one dunder method (__init__) are my own work. 
