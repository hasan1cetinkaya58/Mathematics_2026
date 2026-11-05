A = [[1, 2, 0], [0, 1, 1]]

B = [[1, 0], [2, 1], [-1, 3]]

C = [[2, 1], [0, -1]]

Compute (AB)C:
First calculate AB:

AB = [[1, 2, 0], [0, 1, 1]]

 ×

 [[1, 0],
  [2, 1],
  [-1, 3]]
AB = [[5, 2], [1, 4]]

Now calculate (AB)C:

(AB)C = [[5, 2], [1, 4]]

    ×

    [[2, 1],
     [0, -1]]
(AB)C = [[10, 3], [2, -3]]

Compute A(BC):
First calculate BC:

BC = [[1, 0], [2, 1], [-1, 3]]

 ×

 [[2, 1],
  [0, -1]]
BC = [[2, 1], [4, 1], [-2, -4]]

Now calculate A(BC):

A(BC) = [[1, 2, 0], [0, 1, 1]]

    ×

    [[2, 1],
     [4, 1],
     [-2, -4]]
A(BC) = [[10, 3], [2, -3]]

Compare the results:
(AB)C = [[10, 3], [2, -3]]

A(BC) = [[10, 3], [2, -3]]

Therefore:

(AB)C = A(BC)

Explanation:

Matrix multiplication is associative. Changing the grouping of the matrices does not change the final result.

However, the number of calculations can differ depending on the order of multiplication. In this example, calculating (AB)C requires fewer scalar multiplications than calculating A(BC).

This demonstrates why choosing an efficient calculation path is important.
