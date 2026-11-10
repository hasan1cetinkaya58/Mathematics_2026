
# Exercise 1: Determinant of a 2×2 Matrix

## Question

Compute the determinants of the following matrices:

$$
A=
\begin{pmatrix}
3 & -2\\
5 & 4
\end{pmatrix}
$$

$$
B=
\begin{pmatrix}
1 & 7\\
2 & 14
\end{pmatrix}
$$

Determine which matrix is invertible and justify your answer.

## Solution

### 1. Recall the 2×2 Determinant Formula

For a general 2×2 matrix:

$$
M=
\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
$$

The determinant is calculated using:

$$
\det(M)=ad-bc
$$

We multiply the entries of the main diagonal and subtract the product of the entries of the other diagonal.

### 2. Calculate the Determinant of Matrix A

Given:

$$
A=
\begin{pmatrix}
3 & -2\\
5 & 4
\end{pmatrix}
$$

Applying the determinant formula:

$$
\det(A)=3\cdot4-(-2)\cdot5
$$

Calculating the products:

$$
\det(A)=12-(-10)
$$

Therefore:

$$
\boxed{\det(A)=22}
$$

### 3. Calculate the Determinant of Matrix B

Given:

$$
B=
\begin{pmatrix}
1 & 7\\
2 & 14
\end{pmatrix}
$$

Applying the determinant formula:

$$
\det(B)=1\cdot14-7\cdot2
$$

Calculating the products:

$$
\det(B)=14-14
$$

Therefore:

$$
\boxed{\det(B)=0}
$$

### 4. Determine Which Matrix Is Invertible

A square matrix is invertible if and only if its determinant is non-zero.

The condition for invertibility is:

$$
\det(M)\neq0
$$

For matrix A:

$$
\det(A)=22\neq0
$$

Therefore, matrix A is invertible.

For matrix B:

$$
\det(B)=0
$$

Therefore, matrix B is not invertible. It is a singular matrix.

### 5. Final Conclusion

The calculated determinants are:

$$
\det(A)=22
$$

$$
\det(B)=0
$$

Since the determinant of A is non-zero, A has an inverse.

Since the determinant of B is zero, B does not have an inverse.

Thus, the final answer is:

$$
\boxed{\text{A is invertible}}
$$

$$
\boxed{\text{B is not invertible}}
$$

This exercise demonstrates that the determinant of a square matrix determines whether the matrix is invertible.
