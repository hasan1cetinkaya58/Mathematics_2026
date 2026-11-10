# 
# Exercise 2: Addition and Scalar Multiplication

## Question

Given the matrices:

$$
A =
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix}
$$

Compute:

1. $A+B$
2. $A-B$
3. $3A-2B$

Explain why matrix addition is possible only for matrices of the same size.

## Solution

### 1. Matrix Addition: $A+B$

Matrix addition is performed by adding corresponding entries in the same positions. Both matrices have the same dimensions, so addition is possible.

$$
A+B =
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5
\end{pmatrix}
$$

Calculating each entry:

$$
A+B =
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A+B =
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
}
$$

### 2. Matrix Subtraction: $A-B$

Matrix subtraction is performed by subtracting corresponding entries in the same positions.

$$
A-B =
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5
\end{pmatrix}
$$

Calculating each entry:

$$
A-B =
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A-B =
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
}
$$

### 3. Scalar Multiplication and Subtraction: $3A-2B$

First, multiply every entry of matrix $A$ by the scalar 3:

$$
3A =
\begin{pmatrix}
3 & 6\\
-3 & 9
\end{pmatrix}
$$

Next, multiply every entry of matrix $B$ by the scalar 2:

$$
2B =
\begin{pmatrix}
8 & -4\\
0 & 10
\end{pmatrix}
$$

Now subtract the corresponding entries of $2B$ from $3A$:

$$
3A-2B =
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10
\end{pmatrix}
$$

Calculating each entry:

$$
3A-2B =
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
3A-2B =
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
}
$$

### 4. Why Must Matrices Have the Same Size for Addition?

Matrix addition is possible only when both matrices have the same number of rows and columns.

This is because matrix addition is performed by adding corresponding entries in the same positions.

For example, a $2\times2$ matrix can be added to another $2\times2$ matrix because every entry has a corresponding entry in the other matrix.

However, a $2\times2$ matrix cannot be added to a $2\times3$ matrix because their entries do not have matching positions.

Therefore, matrices must have the same dimensions for addition to be defined.

## Final Answers

$$
\boxed{
A+B =
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
}
$$

$$
\boxed{
A-B =
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
}
$$

$$
\boxed{
3A-2B =
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
}
$$

All three calculations are correct. Since both matrices have dimensions $2\times2$, matrix addition and subtraction are defined.
