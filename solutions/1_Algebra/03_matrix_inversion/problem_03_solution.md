
# Exercise 3: When Does the Inverse Not Exist?

## Question

For

$$
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
$$

Explain in two ways why \(A^{-1}\) does not exist:
using the determinant and using dependence between the rows.

## Solution

### Step 1. Calculate the Determinant

First, we calculate the determinant of matrix \(A\).

For a \(2 \times 2\) matrix, the determinant is calculated using the formula:

$$
\det(A) = ad - bc
$$

Substituting the values from the matrix:

$$
\det(A) =
\begin{vmatrix}
2 & 4 \\
1 & 2
\end{vmatrix}
$$

$$
\det(A) = (2)(2) - (4)(1)
$$

$$
\det(A) = 4 - 4
$$

$$
\boxed{\det(A) = 0}
$$

Since the determinant is zero, the matrix is singular and its inverse does not exist.

### Step 2. Check the Dependence Between the Rows

Now, we examine the relationship between the two rows of matrix \(A\).

The first row is:

$$
R_1 = (2,4)
$$

The second row is:

$$
R_2 = (1,2)
$$

We can see that the second row is exactly half of the first row.

$$
R_2 = \frac{1}{2}R_1
$$

Checking:

$$
\frac{1}{2}(2,4) = (1,2)
$$

Therefore, the rows are linearly dependent.

This means that the rows do not provide independent information, and the matrix does not have full rank.

### Step 3. Explain Why the Inverse Does Not Exist

A square matrix is invertible only if its determinant is nonzero and its rows are linearly independent.

For matrix \(A\):

$$
\det(A) = 0
$$

and

$$
R_2 = \frac{1}{2}R_1
$$

Both conditions show that the matrix is singular.

Therefore, no inverse matrix exists.

### Final Answer

$$
\boxed{\det(A)=0}
$$

$$
\boxed{R_2=\frac{1}{2}R_1}
$$

$$
\boxed{A^{-1}\text{ does not exist}}
$$

### Conclusion

The inverse of matrix \(A\) does not exist for two reasons.

First, its determinant is zero. Second, its rows are linearly dependent because the second row is half of the first row.

These two properties describe the same mathematical problem: the matrix is singular and cannot be inverted.
