
# Exercise 13. Undoing a Composite Transformation

## Question

The matrices

```math
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

describe nonuniform scaling and shear.

For `T = HS`, find `T^(-1)` in two ways:

1. First compute `T`, then its inverse.
2. Use the property `(HS)^(-1) = S^(-1)H^(-1)`.

Compare the results. Additionally, compute `H^(-1)S^(-1)` and verify that the incorrect order gives a different matrix.

Explain the rule: "When undoing a composition of operations, we undo them from the end."

## Solution

### Step 1. Calculate T = HS

We are given:

```math
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
```

Since `T = HS`, we multiply `H` by `S` in this order:

```math
T = HS =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
```

Multiplying the matrices:

```math
T =
\begin{pmatrix}
1\cdot2+1\cdot0 & 1\cdot0+1\cdot1 \\
0\cdot2+1\cdot0 & 0\cdot0+1\cdot1
\end{pmatrix}
```

Therefore:

```math
T =
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
```

### Step 2. Find the Inverse of T Directly

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

First, calculate the determinant of `T`:

```math
\det(T) = 2\cdot1-1\cdot0=2
```

Since the determinant is nonzero, the inverse exists.

Applying the inverse formula:

```math
T^{-1}
=
\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
```

Thus:

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
```

### Step 3. Find the Inverse Using the Product Property

We use the inverse of a product property:

```math
(HS)^{-1}=S^{-1}H^{-1}
```

First, calculate the inverse of `S`:

```math
S^{-1}
=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
```

Next, calculate the inverse of `H`:

```math
H^{-1}
=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
```

Now multiply `S^(-1)` by `H^(-1)` in the correct order:

```math
T^{-1}=S^{-1}H^{-1}
```

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
```

Multiplying the matrices:

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2}\cdot1+0\cdot0 &
\frac{1}{2}\cdot(-1)+0\cdot1 \\
0\cdot1+1\cdot0 &
0\cdot(-1)+1\cdot1
\end{pmatrix}
```

Therefore:

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
```

### Step 4. Compare the Two Results

The first method gives:

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
```

The second method gives:

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
```

Both methods produce exactly the same result.

Therefore, the inverse product property is verified.

### Step 5. Calculate the Incorrect Order

Now calculate `H^(-1)S^(-1)` instead of `S^(-1)H^(-1)`:

```math
H^{-1}S^{-1}
=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
```

Multiplying the matrices:

```math
H^{-1}S^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
```

This is different from the correct inverse:

```math
S^{-1}H^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
```

Therefore:

```math
H^{-1}S^{-1} \neq S^{-1}H^{-1}
```

The order of matrix multiplication matters.

### Step 6. Explain the Rule

The original transformation is:

```math
T=HS
```

This means that the scaling transformation `S` is applied first, followed by the shear transformation `H`.

To undo the complete transformation, we must undo the shear first and then undo the scaling.

Therefore, the inverse is:

```math
T^{-1}=S^{-1}H^{-1}
```

We reverse the order of the transformations when finding the inverse.

### Final Answer

The correct inverse is:

```math
T^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
```

The incorrect order gives:

```math
H^{-1}S^{-1}
=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
```

These two matrices are different.

### Conclusion

The inverse of a product of matrices reverses the order of multiplication:

```math
(HS)^{-1}=S^{-1}H^{-1}
```

This means that when undoing a composition of operations, we must undo the last operation first.

The two correct methods give the same inverse, while reversing the order incorrectly produces a different matrix.
