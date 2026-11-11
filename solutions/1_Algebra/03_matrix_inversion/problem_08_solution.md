
# Exercise 8. Inverse of a Transformation


## Question

The matrix describes a scaling of the plane:

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

Find the inverse matrix $S^{-1}$ and explain geometrically what the inverse transformation does.

Check the action of $S$ followed by $S^{-1}$ on one simple vector.

## Solution

### Step 1. Find the Determinant of S

We calculate the determinant:

$$
\det(S)=
2\cdot\frac{1}{2}-0\cdot0
$$

$$
\det(S)=1
$$

Since the determinant is not zero, the inverse exists.

### Step 2. Calculate the Inverse Matrix

We use the inverse formula for a 2×2 matrix:

$$
S^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
$$

Substituting the values:

$$
S^{-1}=
\frac{1}{1}
\begin{pmatrix}
\frac{1}{2}&0\\
0&2
\end{pmatrix}
$$

### Step 3. Write the Inverse Matrix

Therefore:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2}&0\\
0&2
\end{pmatrix}
$$

### Step 4. Explain the Geometric Meaning

The original transformation stretches the x-coordinate by a factor of 2 and compresses the y-coordinate by a factor of 1/2.

The inverse transformation does the opposite:

- It compresses the x-coordinate by a factor of 1/2.
- It stretches the y-coordinate by a factor of 2.

Therefore, the inverse transformation restores the original size and position of every vector.

### Step 5. Check the Transformation Using a Vector

We choose a simple vector:

$$
v=
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

First, we apply the transformation S:

$$
Sv=
\begin{pmatrix}
2&0\\
0&\frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

Calculation:

$$
Sv=
\begin{pmatrix}
2\cdot1+0\cdot2\\
0\cdot1+\frac{1}{2}\cdot2
\end{pmatrix}
$$

$$
Sv=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

Next, we apply the inverse transformation:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2}&0\\
0&2
\end{pmatrix}
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

Calculation:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2}\cdot2+0\cdot1\\
0\cdot2+2\cdot1
\end{pmatrix}
$$

$$
S^{-1}(Sv)=
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

### Step 6. Final Verification

The original vector is recovered:

$$
S^{-1}(Sv)=v
$$

We can also verify the matrices:

$$
SS^{-1}=
\begin{pmatrix}
2&0\\
0&\frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2}&0\\
0&2
\end{pmatrix}
$$

$$
SS^{-1}=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
$$

### Final Answer

$$
\boxed{
S^{-1}=
\begin{pmatrix}
\frac{1}{2}&0\\
0&2
\end{pmatrix}
}
$$

### Conclusion

The inverse transformation reverses the original scaling. It compresses the x-coordinate by 1/2 and stretches the y-coordinate by 2.

Applying the inverse transformation after the original transformation returns every vector to its initial position.
