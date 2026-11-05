Columns of a Matrix Product
Given:

A = [[1, 2, 0], [0, 1, 1]]

B = [[1, 2], [-1, 0], [3, 1]]

The columns of B are:

b1 = [[1], [-1], [3]]

b2 = [[2], [0], [1]]

Compute Ab1 and Ab2:
Ab1 = [[1, 2, 0], [0, 1, 1]] × [[1], [-1], [3]]

Ab1 = [[1 - 2 + 0], [-1 + 3]]

Ab1 = [[-1], [2]]

Ab2 = [[1, 2, 0], [0, 1, 1]] × [[2], [0], [1]]

Ab2 = [[2 + 0 + 0], [0 + 1]]

Ab2 = [[2], [1]]

Compute AB:
AB = [[-1, 2], [2, 1]]

Comparison:
The columns of AB are exactly the vectors Ab1 and Ab2. This shows that matrix multiplication can be understood as applying matrix A to each column of matrix B.
