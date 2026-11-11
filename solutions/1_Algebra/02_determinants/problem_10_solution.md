# Exercise 10 – Detecting Dependence

## Question

Given the matrix:

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 4 & 6\\
0 & 1 & 5
\end{pmatrix}
$$

Explain why the determinant is zero without carrying out a full determinant calculation.

1. Identify the specific rows that are linearly dependent and explain the relationship between them.
2. Explain why this row dependence makes the determinant zero.
3. Explain how this implies that the matrix is not invertible.

## Solution

### 1. Identify the Dependence Between the Rows

Consider the first and second rows:

$$
R_1=(1,2,3)
$$

$$
R_2=(2,4,6)
$$

We can see that the second row is exactly twice the first row:

$$
R_2=2R_1
$$

Therefore, the first and second rows are linearly dependent.

### 2. Why Does This Make the Determinant Zero?

A fundamental property of determinants states that if two rows of a square matrix are linearly dependent, its determinant must be zero.

In this matrix, the second row is a multiple of the first row. Therefore, the rows do not provide three independent directions.

Consequently:

$$
\det(A)=0
$$

### 3. Connection with Noninvertibility

A square matrix is invertible if and only if its determinant is nonzero.

Since:

$$
\det(A)=0
$$

the matrix is not invertible.

This means that the matrix has no inverse.

The row dependence explains why the determinant is zero and, as a result, why the matrix is singular.

### 4. Final Conclusion

The determinant is zero because the second row is twice the first row:

$$
R_2=2R_1
$$

This makes the rows linearly dependent. Therefore, the determinant is zero, and the matrix is not invertible.

**Final Answer:**

$$
\boxed{\det(A)=0}
$$

The matrix is singular (not invertible) because its rows are linearly dependent.
