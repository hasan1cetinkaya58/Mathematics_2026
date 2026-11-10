
# Exercise 10 – Detecting Dependence

## 1. Given Matrix

The determinant is given as:

$$
\det(A)=
\det\begin{pmatrix}
1 & 2 & 3\\
2 & 4 & 6\\
0 & 1 & 5
\end{pmatrix}
$$

We are asked to explain why the determinant is zero without carrying out a full determinant calculation.

## 2. Identify the Dependence Between the Rows

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

Therefore, the rows are linearly dependent.

## 3. Why Does This Make the Determinant Zero?

A fundamental property of determinants states that if two rows of a square matrix are linearly dependent, its determinant must be zero.

In this matrix, the second row is a multiple of the first row. Therefore, the rows do not provide three independent directions.

Consequently:

$$
\det(A)=0
$$

## 4. Connection with Noninvertibility

A square matrix is invertible if and only if its determinant is nonzero.

Since:

$$
\det(A)=0
$$

the matrix is not invertible.

This means that the matrix has no inverse.

## 5. Final Conclusion

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
