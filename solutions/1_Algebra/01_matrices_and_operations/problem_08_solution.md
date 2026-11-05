Row Operations and Their Reversibility
Given:

A = [[1, 2, -1], [2, 4, 1], [-1, 1, 3]]

Step 1: R2 ← R2 - 2R1

R2 = [2, 4, 1] - 2[1, 2, -1]

R2 = [0, 0, 3]

Matrix after Step 1:

[[1, 2, -1], [0, 0, 3], [-1, 1, 3]]

Reverse operation:

R2 ← R2 + 2R1

Step 2: R3 ← R3 + R1

R3 = [-1, 1, 3] + [1, 2, -1]

R3 = [0, 3, 2]

Matrix after Step 2:

[[1, 2, -1], [0, 0, 3], [0, 3, 2]]

Reverse operation:

R3 ← R3 - R1

Step 3: Interchange R2 and R3

Matrix after Step 3:

[[1, 2, -1], [0, 3, 2], [0, 0, 3]]

Reverse operation:

Interchange R2 and R3 again.

Explanation:

All three row operations are reversible. Each operation has an inverse that restores the original matrix.

