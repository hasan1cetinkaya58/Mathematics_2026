
# Exercise 14. A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix `A` satisfies:

```math
A^2 = I
```

Show that:

```math
A^{-1} = A
```

Then give an example of a `2 × 2` matrix different from `I` and `-I` that satisfies this condition, and verify it by multiplication.

## Solution

### Step 1. Understand the Given Condition

We are given:

```math
A^2 = I
```

By the definition of matrix powers:

```math
A \cdot A = I
```

This means that multiplying matrix `A` by itself gives the identity matrix.

### Step 2. Show That A Is Its Own Inverse

The definition of an inverse matrix states that a matrix multiplied by its inverse gives the identity matrix:

```math
A \cdot A^{-1} = I
```

From the given condition, we also know that:

```math
A \cdot A = I
```

Comparing these two equations, we see that `A` itself satisfies the definition of the inverse of `A`.

Therefore:

```math
A^{-1} = A
```

This proves that the matrix is its own inverse.

### Step 3. Construct a 2 × 2 Example

We choose the following matrix:

```math
A =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
```

This matrix is different from both identity matrices `I` and `-I`.

The identity matrix is:

```math
I =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
```

The negative identity matrix is:

```math
-I =
\begin{pmatrix}
-1 & 0 \\
0 & -1
\end{pmatrix}
```

Our chosen matrix is different from both.

### Step 4. Verify the Condition by Multiplication

We need to check whether:

```math
A^2 = I
```

Using our chosen matrix:

```math
A^2 = A \cdot A
```

Substituting the matrix:

```math
A^2 =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
```

Multiplying the matrices:

```math
A^2 =
\begin{pmatrix}
0\cdot0+1\cdot1 & 0\cdot1+1\cdot0 \\
1\cdot0+0\cdot1 & 1\cdot1+0\cdot0
\end{pmatrix}
```

Simplifying:

```math
A^2 =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
```

Therefore:

```math
A^2 = I
```

The condition is satisfied.

### Step 5. Verify That A Is Its Own Inverse

Since we have shown that:

```math
A \cdot A = I
```

it follows that:

```math
A^{-1} = A
```

Therefore:

```math
A^{-1} =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
```

The multiplication confirms that the chosen matrix is its own inverse.

### Final Answer

For every square matrix satisfying `A^2 = I`:

```math
A^{-1} = A
```

One valid example is:

```math
A =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
```

Its square is:

```math
A^2 =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
```

Therefore, the example satisfies the required condition.

### Conclusion

A square matrix whose square is the identity matrix is equal to its own inverse.

The example demonstrates that a matrix different from both `I` and `-I` can also satisfy this property.

The multiplication verification confirms that the result is correct.
