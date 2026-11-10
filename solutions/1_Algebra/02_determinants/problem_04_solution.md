
# Exercise 4: Triangular Matrix

## Question

Given the matrix:

$$
A=
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
$$

Compute the determinant without expanding it. State the rule for an arbitrary triangular matrix and explain it using this example.

## Solution

### 1. Identify the Type of Matrix

The given matrix is an upper triangular matrix because all entries below the main diagonal are zero.

$$
A=
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
$$

The main diagonal entries are:

$$
2,\quad -3,\quad 7
$$

### 2. Apply the Triangular Matrix Determinant Rule

The determinant of a triangular matrix is equal to the product of its main diagonal entries.

$$
\det(A)=2\cdot(-3)\cdot7
$$

First:

$$
2\cdot(-3)=-6
$$

Then:

$$
-6\cdot7=-42
$$

Therefore:

$$
\boxed{\det(A)=-42}
$$

### 3. State the General Rule

For any upper or lower triangular matrix, the determinant is equal to the product of all entries on its main diagonal.

For an arbitrary n x n triangular matrix:

$$
A=
\begin{pmatrix}
a_{11} & * & \cdots & * \\
0 & a_{22} & \cdots & * \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & a_{nn}
\end{pmatrix}
$$

The general formula is:

$$
\boxed{\det(A)=a_{11}a_{22}\cdots a_{nn}}
$$

The same rule applies to lower triangular matrices.

### 4. Explain the Result Using This Example

In our example, all entries below the main diagonal are zero.

Therefore, we do not need to expand the determinant or use Sarrus' rule.

We simply multiply the diagonal entries:

$$
\det(A)=2\cdot(-3)\cdot7=-42
$$

The result is negative because there is one negative diagonal entry.

## Final Conclusion

The determinant of the given upper triangular matrix is:

$$
\boxed{\det(A)=-42}
$$

This exercise demonstrates that the determinant of any triangular matrix can be calculated directly by multiplying its main diagonal entries, without performing a full determinant expansion.
