
# Exercise 1: Matrix Size and Entries

## Given

The following matrices are given:

$$
A =
\begin{bmatrix}
2 & -1 & 3 \\
0 & 4 & 5
\end{bmatrix}
$$

$$
B =
\begin{bmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1
\end{bmatrix}
$$

## Tasks

1. State the sizes of matrices A and B.
2. Find the entries a₁₂, a₂₃, b₂₁, and b₃₂.
3. Write the second row of A and the first column of B as vectors.

## Solution

### Step 1: Determine the Dimensions of the Matrices

The dimensions of a matrix are determined by counting its rows and columns.

Matrix A has 2 rows and 3 columns. Therefore:

$$
\boxed{\dim(A)=2\times3}
$$

Matrix B has 3 rows and 2 columns. Therefore:

$$
\boxed{\dim(B)=3\times2}
$$

### Step 2: Find the Requested Matrix Entries

In matrix notation, the first index represents the row, and the second index represents the column.

For matrix A:

- The element a₁₂ is in row 1, column 2.

$$
\boxed{a_{12}=-1}
$$

- The element a₂₃ is in row 2, column 3.

$$
\boxed{a_{23}=5}
$$

For matrix B:

- The element b₂₁ is in row 2, column 1.

$$
\boxed{b_{21}=-2}
$$

- The element b₃₂ is in row 3, column 2.

$$
\boxed{b_{32}=1}
$$

### Step 3: Write the Requested Row and Column as Vectors

The second row of matrix A consists of the elements in its second row:

$$
\boxed{
\begin{bmatrix}
0 & 4 & 5
\end{bmatrix}
}
$$

The first column of matrix B consists of the elements in its first column:

$$
\boxed{
\begin{bmatrix}
1\\
-2\\
4
\end{bmatrix}
}
$$

### Step 4: Verification

We can verify the results by checking the positions of the elements in the original matrices.

- In A, row 1 and column 2 contain -1.
- In A, row 2 and column 3 contain 5.
- In B, row 2 and column 1 contain -2.
- In B, row 3 and column 2 contain 1.

The second row of A is [0, 4, 5], and the first column of B is [1, -2, 4]ᵀ.

All the results are consistent with the given matrices.

## Final Answer

- Dimension of A: 2 × 3
- Dimension of B: 3 × 2
- a₁₂ = -1
- a₂₃ = 5
- b₂₁ = -2
- b₃₂ = 1
- Second row of A: [0, 4, 5]
- First column of B: [1, -2, 4]ᵀ
