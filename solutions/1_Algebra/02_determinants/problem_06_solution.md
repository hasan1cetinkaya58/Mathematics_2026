
# Exercise 6: Parameter and Invertibility

## Question

Given the matrix:

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
$$

Find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

## Solution

### 1. Recall the Invertibility Condition

A square matrix is invertible if and only if its determinant is non-zero.

Therefore, a matrix is not invertible when its determinant equals zero.

We use the condition:

$$
\det(A(t))=0
$$

### 2. Calculate the Determinant

For a $2\times2$ matrix, the determinant formula is:

$$
\det(A)=ad-bc
$$

We are given:

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
$$

Applying the formula:

$$
\det(A(t))=t\cdot t-1\cdot2
$$

Simplifying:

$$
\det(A(t))=t^2-2
$$

### 3. Find the Values of t

The matrix is not invertible when its determinant is zero.

Therefore:

$$
t^2-2=0
$$

Adding 2 to both sides:

$$
t^2=2
$$

Taking the square root of both sides:

$$
t=\pm\sqrt{2}
$$

Thus, the two solutions are:

$$
t=\sqrt{2}
$$

and

$$
t=-\sqrt{2}
$$

### 4. Explain the Relationship with Invertibility

The determinant determines whether the matrix has an inverse.

- If $t\neq\pm\sqrt{2}$, the determinant is non-zero, so the matrix is invertible.
- If $t=\sqrt{2}$ or $t=-\sqrt{2}$, the determinant is zero, so the matrix is not invertible.

### 5. Final Conclusion

The determinant of the given matrix is:

$$
\det(A(t))=t^2-2
$$

Setting the determinant equal to zero gives:

$$
t^2-2=0
$$

Therefore, the matrix is not invertible precisely when:

$$
\boxed{t\in\{-\sqrt{2},\sqrt{2}\}}
$$

For all other real values of $t$, the matrix is invertible.
