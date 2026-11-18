
# Exercise 11. Parameter and Invertibility

## Question

For the matrix:

```math
A(t)=
\begin{pmatrix}
1 & t\\
t & 1
\end{pmatrix}
```

Find all values of $t$ for which the matrix is invertible. Then give a formula for $A(t)^{-1}$.

Explain what happens to this formula at the excluded values.

## Solution

### Step 1. Calculate the Determinant

A square matrix is invertible if and only if its determinant is nonzero.

```math
\det(A(t))=
\begin{vmatrix}
1 & t\\
t & 1
\end{vmatrix}
```

```math
=1\cdot1-t\cdot t
```

```math
=1-t^2
```

Factorizing:

```math
\boxed{\det(A(t))=(1-t)(1+t)}
```

### Step 2. Determine the Values of t

The matrix is invertible if:

```math
\det(A(t))\neq0
```

Therefore:

```math
1-t^2\neq0
```

```math
t^2\neq1
```

```math
(t-1)(t+1)\neq0
```

Thus:

```math
\boxed{t\neq1,\quad t\neq-1}
```

The matrix is invertible for all real values of $t$ except $1$ and $-1$.

### Step 3. Find the Inverse Matrix

For a two-by-two matrix:

```math
A=
\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
```

The inverse formula is:

```math
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b\\
-c & a
\end{pmatrix}
```

For the given matrix:

```math
A(t)=
\begin{pmatrix}
1 & t\\
t & 1
\end{pmatrix}
```

We have:

```math
a=1,\quad b=t,\quad c=t,\quad d=1
```

Substituting:

```math
A(t)^{-1}=
\frac{1}{1\cdot1-t\cdot t}
\begin{pmatrix}
1 & -t\\
-t & 1
\end{pmatrix}
```

Therefore:

```math
\boxed{
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t\\
-t & 1
\end{pmatrix}
}
```

This formula is valid when:

```math
t\neq1,\quad t\neq-1
```

### Step 4. Explain What Happens at the Excluded Values

First, consider $t=1$.

```math
A(1)=
\begin{pmatrix}
1 & 1\\
1 & 1
\end{pmatrix}
```

Its determinant is:

```math
\det(A(1))=1-1^2=0
```

The two rows are identical. Therefore, the matrix is not invertible.

Now, consider $t=-1$.

```math
A(-1)=
\begin{pmatrix}
1 & -1\\
-1 & 1
\end{pmatrix}
```

Its determinant is:

```math
\det(A(-1))=1-(-1)^2=0
```

The second row is the negative of the first row. Therefore, this matrix is also not invertible.

At both excluded values, the denominator becomes zero:

```math
1-t^2=0
```

Division by zero is undefined. Therefore, the inverse does not exist at $t=1$ or $t=-1$.

### Step 5. Verify the Inverse Formula

We verify the proposed inverse by multiplying $A(t)$ by $A(t)^{-1}$.

```math
A(t)A(t)^{-1}
```

Substituting the matrices:

```math
=
\begin{pmatrix}
1 & t\\
t & 1
\end{pmatrix}
\cdot
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t\\
-t & 1
\end{pmatrix}
```

Multiplying the matrices:

```math
=
\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & -t+t\\
t-t & 1-t^2
\end{pmatrix}
```

Simplifying:

```math
=
\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & 0\\
0 & 1-t^2
\end{pmatrix}
```

Therefore:

```math
\boxed{
A(t)A(t)^{-1}=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
=I_2
}
```

This confirms that the inverse formula is correct for $t\neq1$ and $t\neq-1$.

## Final Answer

The matrix is invertible for all real values except $-1$ and $1$.

```math
\boxed{t\in\mathbb{R}\setminus\{-1,1\}}
```

The inverse matrix is:

```math
\boxed{
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t\\
-t & 1
\end{pmatrix}
}
```

The inverse does not exist at:

```math
\boxed{t=-1\quad\text{or}\quad t=1}
```

## Conclusion

The invertibility of $A(t)$ depends on the value of the parameter $t$.

For all real values except $t=-1$ and $t=1$, the determinant is nonzero and the inverse exists.

At $t=-1$ and $t=1$, the determinant is zero because the rows are linearly dependent. Therefore, the inverse does not exist.

> **Why this exercise:** This exercise combines a parameter, determinant calculation, and an explicit inverse formula in one problem.
