
# Exercise 11. Parameter and Invertibility

## Question

For the matrix

```math
A(t) =
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
```

Find all values of `t` for which the matrix is invertible. Then give a formula for `A(t)^(-1)`.

Explain what happens to this formula at the excluded values.

## Solution

### Step 1. Calculate the Determinant

A square matrix is invertible if and only if its determinant is nonzero.

For the given matrix:

```math
\det(A(t)) = 1 \cdot 1 - t \cdot t
```

Simplifying:

```math
\det(A(t)) = 1 - t^2
```

Factorizing:

```math
\det(A(t)) = (1-t)(1+t)
```

### Step 2. Determine the Values of t

The matrix is invertible if its determinant is not zero:

```math
1-t^2 \neq 0
```

Therefore:

```math
t^2 \neq 1
```

This means:

```math
t \neq 1
```

and

```math
t \neq -1
```

Thus, the matrix is invertible for all real values of `t` except `1` and `-1`.

### Step 3. Find the Inverse Matrix

For a two-by-two matrix, the inverse formula is:

```math
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}^{-1}
=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
```

Applying this formula to `A(t)`:

```math
A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
```

This formula is valid only when `t` is different from `1` and `-1`.

### Step 4. Explain What Happens at the Excluded Values

First, consider `t = 1`:

```math
A(1) =
\begin{pmatrix}
1 & 1 \\
1 & 1
\end{pmatrix}
```

The two rows are identical. Therefore, the determinant is zero and the matrix is not invertible.

Now, consider `t = -1`:

```math
A(-1) =
\begin{pmatrix}
1 & -1 \\
-1 & 1
\end{pmatrix}
```

The second row is the negative of the first row. Therefore, the determinant is also zero and the matrix is not invertible.

At both excluded values, the denominator of the inverse formula becomes zero:

```math
1-t^2 = 0
```

Division by zero is undefined. Therefore, the inverse does not exist at `t = 1` or `t = -1`.

### Step 5. Verify the Inverse Formula

We verify the proposed inverse by multiplying `A(t)` by `A(t)^(-1)`:

```math
A(t)A(t)^{-1}
=
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
```

Multiplying the matrices:

```math
A(t)A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & -t+t \\
t-t & 1-t^2
\end{pmatrix}
```

Simplifying:

```math
A(t)A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & 0 \\
0 & 1-t^2
\end{pmatrix}
```

Therefore:

```math
A(t)A(t)^{-1}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
```

This confirms that the inverse formula is correct for `t` different from `1` and `-1`.

### Final Answer

The matrix is invertible for all real values of `t` except `-1` and `1`:

```math
t \in \mathbb{R} \setminus \{-1,1\}
```

The inverse matrix is:

```math
A(t)^{-1}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
```

This formula is valid when `t` is different from `-1` and `1`.

### Conclusion

The invertibility of `A(t)` depends on the value of the parameter `t`.

For all real values except `t = -1` and `t = 1`, the determinant is nonzero and the inverse exists.

At `t = -1` and `t = 1`, the determinant is zero because the rows are linearly dependent. Therefore, the inverse does not exist.
