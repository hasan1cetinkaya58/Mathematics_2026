
# Exercise 12. Finding Inverses Without Starting from Scratch

## Question

It is known that

```math
A^{-1} =
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
```

Without finding `A`, compute `(3A)^(-1)`, `(A^T)^(-1)`, and `(A^2)^(-1)`.

Justify each result using the appropriate property.

## Solution

### Step 1. Calculate the Inverse of 3A

We use the scalar multiplication property of inverse matrices:

```math
(cA)^{-1} = \frac{1}{c}A^{-1}
```

Since the scalar is `3`, we obtain:

```math
(3A)^{-1} = \frac{1}{3}A^{-1}
```

Substituting the given inverse:

```math
(3A)^{-1}
=
\frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
```

Therefore:

```math
(3A)^{-1}
=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3}
\end{pmatrix}
```

### Step 2. Calculate the Inverse of A Transpose

We use the transpose property:

```math
(A^T)^{-1} = (A^{-1})^T
```

This means we transpose the given inverse matrix by switching its rows and columns:

```math
(A^T)^{-1}
=
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}
```

### Step 3. Calculate the Inverse of A Squared

We use the power property of inverse matrices:

```math
(A^2)^{-1} = (A^{-1})^2
```

Therefore:

```math
(A^2)^{-1}
=
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
```

Multiplying the matrices:

```math
(A^2)^{-1}
=
\begin{pmatrix}
2\cdot2+(-1)\cdot(-3) & 2\cdot(-1)+(-1)\cdot2 \\
(-3)\cdot2+2\cdot(-3) & (-3)\cdot(-1)+2\cdot2
\end{pmatrix}
```

Simplifying:

```math
(A^2)^{-1}
=
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}
```

### Final Answer

The three results are:

**1. Inverse of 3A**

```math
(3A)^{-1}
=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3}
\end{pmatrix}
```

**2. Inverse of A Transpose**

```math
(A^T)^{-1}
=
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}
```

**3. Inverse of A Squared**

```math
(A^2)^{-1}
=
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}
```

### Conclusion

We used three important properties of inverse matrices:

1. The inverse of a scalar multiple is the inverse matrix multiplied by the reciprocal of the scalar.

2. The inverse of a transpose is the transpose of the inverse.

3. The inverse of a matrix power is the corresponding power of the inverse matrix.

These properties allow us to calculate all three results without finding the original matrix `A`.
