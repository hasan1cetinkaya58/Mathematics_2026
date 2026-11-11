
# Exercise 15. Two Methods for Solving the Same System

## Question

For

```math
A =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
b =
\begin{pmatrix}
7 \\
8
\end{pmatrix}
```

Solve `Ax = b` in two ways:

1. Using `A^(-1)b`.
2. Using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

### Method 1. Using the Inverse Matrix

### Step 1. Calculate the Determinant of A

First, we calculate the determinant to check whether the inverse exists.

```math
\det(A) =
\begin{vmatrix}
2 & 1 \\
1 & 3
\end{vmatrix}
```

Calculation:

```math
\det(A) = 2 \cdot 3 - 1 \cdot 1
```

```math
\det(A) = 6 - 1 = 5
```

Since the determinant is not zero, the inverse of A exists.

### Step 2. Find the Inverse of A

We use the inverse formula for a 2×2 matrix:

```math
A^{-1} =
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
```

Substituting the values:

```math
A^{-1} =
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
```

Therefore:

```math
A^{-1} =
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
```

### Step 3. Calculate x Using x = A⁻¹b

We use the formula:

```math
x = A^{-1}b
```

Substituting the matrices:

```math
x =
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
\begin{pmatrix}
7 \\
8
\end{pmatrix}
```

Calculation:

```math
x =
\begin{pmatrix}
\frac{3}{5}\cdot 7 - \frac{1}{5}\cdot 8 \\
-\frac{1}{5}\cdot 7 + \frac{2}{5}\cdot 8
\end{pmatrix}
```

```math
x =
\begin{pmatrix}
\frac{21}{5}-\frac{8}{5} \\
-\frac{7}{5}+\frac{16}{5}
\end{pmatrix}
```

Therefore:

```math
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
```

The solution using the inverse matrix method is:

```math
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
```

## Method 2. Using Gaussian Elimination

### Step 4. Construct the Augmented Matrix

We start with the equation `Ax = b` and write the augmented matrix.

```math
[A \mid b] =
\left[
\begin{array}{cc|c}
2 & 1 & 7 \\
1 & 3 & 8
\end{array}
\right]
```

### Step 5. Eliminate the First Entry in the Second Row

We apply the row operation:

```math
R_2 \rightarrow 2R_2 - R_1
```

Calculation:

```math
2(1,3,8)-(2,1,7)
```

```math
R_2 = (0,5,9)
```

The new augmented matrix becomes:

```math
\left[
\begin{array}{cc|c}
2 & 1 & 7 \\
0 & 5 & 9
\end{array}
\right]
```

### Step 6. Make the Second Pivot Equal to 1

We divide the second row by 5.

```math
R_2 \rightarrow \frac{1}{5}R_2
```

The new augmented matrix becomes:

```math
\left[
\begin{array}{cc|c}
2 & 1 & 7 \\
0 & 1 & \frac{9}{5}
\end{array}
\right]
```

### Step 7. Eliminate the Entry Above the Second Pivot

We apply the row operation:

```math
R_1 \rightarrow R_1 - R_2
```

Calculation:

```math
(2,1,7)-
\left(0,1,\frac{9}{5}\right)
```

```math
R_1 =
\left(2,0,\frac{26}{5}\right)
```

The new augmented matrix becomes:

```math
\left[
\begin{array}{cc|c}
2 & 0 & \frac{26}{5} \\
0 & 1 & \frac{9}{5}
\end{array}
\right]
```

### Step 8. Make the First Pivot Equal to 1

We divide the first row by 2.

```math
R_1 \rightarrow \frac{1}{2}R_1
```

The final augmented matrix becomes:

```math
\left[
\begin{array}{cc|c}
1 & 0 & \frac{13}{5} \\
0 & 1 & \frac{9}{5}
\end{array}
\right]
```

Therefore:

```math
x_1 = \frac{13}{5},
\qquad
x_2 = \frac{9}{5}
```

The solution using Gaussian elimination is:

```math
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
```

### Step 9. Compare Both Solutions

The inverse matrix method gives:

```math
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
```

The Gaussian elimination method gives:

```math
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
```

Both methods produce exactly the same solution.

### Step 10. Verify the Result

We substitute the solution into the original equation `Ax = b`.

```math
A x =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
```

Calculation:

```math
Ax =
\begin{pmatrix}
2\cdot\frac{13}{5}+\frac{9}{5} \\
\frac{13}{5}+3\cdot\frac{9}{5}
\end{pmatrix}
```

```math
Ax =
\begin{pmatrix}
\frac{26}{5}+\frac{9}{5} \\
\frac{13}{5}+\frac{27}{5}
\end{pmatrix}
```

```math
Ax =
\begin{pmatrix}
\frac{35}{5} \\
\frac{40}{5}
\end{pmatrix}
```

Therefore:

```math
Ax =
\begin{pmatrix}
7 \\
8
\end{pmatrix}
= b
```

The result matches the original vector b, so the solution is correct.

## Comparison of the Two Methods

### Number of Essential Steps

**Inverse Matrix Method:**

1. Calculate the determinant.
2. Find the inverse matrix.
3. Multiply the inverse matrix by b.

**Gaussian Elimination:**

1. Construct the augmented matrix.
2. Perform row operations to obtain the solution.

Gaussian elimination required four row operations in this solution.

### Which Method Was Simpler?

In this example, Gaussian elimination was simpler because we only needed to solve one system of equations.

The inverse matrix method required calculating the entire inverse matrix before multiplying it by b.

For a single system, Gaussian elimination is more direct. However, the inverse matrix method can be useful when the inverse is already known or when solving several systems with the same matrix A.

## Final Answer

Both methods give the same solution:

```math
\boxed{
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
}
```

## Conclusion

We solved the same linear system using two different methods: the inverse matrix method and Gaussian elimination.

Both methods produced the same solution, and substitution confirmed that the result satisfies the original equation.

In this example, Gaussian elimination was simpler because it required fewer essential calculations and avoided finding the complete inverse matrix.
