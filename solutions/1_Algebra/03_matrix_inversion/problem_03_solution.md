
# Exercise 3: When Does the Inverse Not Exist?

## Question

Consider the following matrix:

$$
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
$$

Explain in two different ways why the inverse matrix $A^{-1}$ does not exist:

1. Using the determinant of the matrix.
2. Using the linear dependence between the rows.

## Solution

### Step 1. Calculate the Determinant

For a $2 \times 2$ matrix, the determinant is calculated using the formula:

$$
\det(A) = ad - bc
$$

The given matrix is:

$$
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
$$

Substituting the values into the formula:

$$
\det(A) = (2)(2) - (4)(1)
$$

$$
\det(A) = 4 - 4
$$

$$
\det(A) = 0
$$

Since the determinant is zero, matrix $A$ is singular. Therefore, its inverse does not exist.

### Step 2. Examine the Linear Dependence Between the Rows

The first row of matrix $A$ is:

$$
R_1 = (2,4)
$$

The second row of matrix $A$ is:

$$
R_2 = (1,2)
$$

We can see that the second row is exactly half of the first row:

$$
R_2 = \frac{1}{2}R_1
$$

To verify this relationship:

$$
\frac{1}{2}(2,4) = (1,2)
$$

Therefore, the two rows are linearly dependent.

### Step 3. Explain Why the Inverse Does Not Exist

A square matrix is invertible if and only if its rows are linearly independent and its determinant is nonzero.

For matrix $A$, we have:

$$
\det(A) = 0
$$

and

$$
R_2 = \frac{1}{2}R_1
$$

The rows are linearly dependent. Therefore, matrix $A$ does not have full rank.

Since the matrix has two rows but only one linearly independent row, its rank is:

$$
\text{rank}(A) = 1
$$

Consequently, matrix $A$ is singular and cannot have an inverse.

### Final Answer

The determinant is:

$$
\boxed{\det(A) = 0}
$$

The rows are linearly dependent:

$$
\boxed{R_2 = \frac{1}{2}R_1}
$$

Therefore:

$$
\boxed{A^{-1} \text{ does not exist}}
$$

### Conclusion

The inverse of matrix $A$ does not exist for two reasons.

First, its determinant is zero. Second, its rows are linearly dependent because the second row is exactly half of the first row.

Both properties show that matrix $A$ is singular and cannot be inverted.
