# DFS_python

The python code traverses a graph using the Depth-Search First (DFS) and displays the provided graph and the resulting DFS path. The user can input a custom graph and specify a starting node for the DFS; a default graph and a default start node are also included.

## Default Graph and DFS path

#### Default Graph

![default-2](https://user-images.githubusercontent.com/20401990/137212602-98844193-bee0-40c2-8758-3b8b1385c834.png)

#### DFS Path for the Default Graph

![default-1](https://user-images.githubusercontent.com/20401990/137212678-3c63870d-1344-4a59-aefe-3138b4a571ea.png)


The steps for traversing using the DFS are as follows (using a stack for suspended nodes):

```
Enter adjacency matrix: Enter 1 to use the default; Enter 2 to input a custom matrix:  1
---Adjacency Matrix---
Node/Row 1 :  [0 1 0 0 0 0 0 0 0 0 0 0 0 0 0]
Node/Row 2 :  [1 0 1 0 0 0 0 0 0 0 0 0 0 0 0]
Node/Row 3 :  [0 1 0 1 1 0 0 0 0 0 0 0 0 0 0]
Node/Row 4 :  [0 0 1 0 0 0 0 0 0 0 0 0 0 0 0]
Node/Row 5 :  [0 0 1 0 0 0 1 0 0 0 0 0 0 0 0]
Node/Row 6 :  [0 0 0 0 0 0 0 0 0 0 0 0 0 0 0]
Node/Row 7 :  [0 0 0 0 1 0 0 1 0 0 0 0 0 1 0]
Node/Row 8 :  [0 0 0 0 0 0 1 0 1 1 0 0 0 0 0]
Node/Row 9 :  [0 0 0 0 0 0 0 0 0 0 1 1 0 0 0]
Node/Row 10 :  [0 0 0 0 0 0 0 1 0 0 0 0 1 0 1]
Node/Row 11 :  [0 0 0 0 0 0 0 0 1 0 0 0 0 0 0]
Node/Row 12 :  [0 0 0 0 0 0 0 0 1 0 0 0 0 0 0]
Node/Row 13 :  [0 0 0 0 0 0 0 0 0 1 0 0 0 0 0]
Node/Row 14 :  [0 0 0 0 0 0 1 0 0 0 0 0 0 0 0]
Node/Row 15 :  [0 0 0 0 0 0 0 0 0 1 0 0 0 0 0]

Enter START node for DFS:  1
--------------- 0
Iteration:  0
Current:  1
Next:  [2]
VISITED:  [1]
STACK:  []
--------------- 1
Iteration:  1
Current:  2
Next:  [3]
VISITED:  [1, 2]
STACK:  []
--------------- 2
Iteration:  2
Current:  3
Next:  [4]
VISITED:  [1, 2, 3]
STACK:  [3]
--------------- 3
Iteration:  3
Current:  4
VISITED:  [1, 2, 3, 4]
STACK:  [3]
--------------- 4
Iteration:  4
current:  3
Next:  [5]
VISITED:  [1, 2, 3, 4]
STACK:  []
--------------- 5
Iteration:  5
current:  5
Next:  [7]
VISITED:  [1, 2, 3, 4, 5]
STACK:  []
--------------- 6
Iteration:  6
Current:  7
Next:  [8]
VISITED:  [1, 2, 3, 4, 5, 7]
STACK:  [7]
--------------- 7
Iteration:  7
Current:  8
Next:  [9]
VISITED:  [1, 2, 3, 4, 5, 7, 8]
STACK:  [7, 8]
--------------- 8
Iteration:  8
Current:  9
Next:  [11]
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9]
STACK:  [7, 8, 9]
--------------- 9
Iteration:  9
current:  11
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11]
STACK:  [7, 8, 9]
--------------- 10
Iteration:  10
Current:  9
Next:  [12]
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11]
STACK:  [7, 8]
--------------- 11
Iteration:  11
Current:  12
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12]
STACK:  [7, 8]
--------------- 12
Iteration:  12
Current:  8
Next:  [10]
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12]
STACK:  [7]
--------------- 13
Iteration:  13
current:  10
Next:  [13]
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12, 10]
STACK:  [7, 10]
--------------- 14
Iteration:  14
current:  13
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12, 10, 13]
STACK:  [7, 10]
--------------- 15
Iteration:  15
Current:  10
Next:  [15]
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12, 10, 13]
STACK:  [7]
--------------- 16
Iteration:  16
Current:  15
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12, 10, 13, 15]
STACK:  [7]
--------------- 17
Iteration:  17
Current:  7
Next:  [14]
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12, 10, 13, 15]
STACK:  []
--------------- 18
Iteration:  18
Current:  14
VISITED:  [1, 2, 3, 4, 5, 7, 8, 9, 11, 12, 10, 13, 15, 14]
STACK:  []


```


## Another example

#### Graph
![2-1](https://user-images.githubusercontent.com/20401990/137213269-5581186c-88f4-4936-8aae-97b7530a0f24.png)



#### DFS Path
![2-2](https://user-images.githubusercontent.com/20401990/137213303-0d60d89b-f05d-4ca1-a36d-089cab8b773d.png)











