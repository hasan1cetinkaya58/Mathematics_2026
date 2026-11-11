
# Exercise 9. Matrix Equation

## Question

Given

$$
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Solve the equation $AX=B$ for $X$.

Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

### Step 1. Determine Where to Apply the Inverse

We are given:

$$
AX=B
$$

Since $A$ is multiplied on the left side of $X$, we must multiply both sides by $A^{-1}$ on the left:

$$
A^{-1}AX=A^{-1}B
$$

Since $A^{-1}A=I$, we obtain:

$$
X=A^{-1}B
$$

### Step 2. Calculate the Inverse of A

First, calculate the determinant:

$$
\det(A)=1\cdot1-2\cdot0=1
$$

Since the determinant is not zero, the inverse exists.

Using the inverse formula:

$$
A^{-1}=
\frac{1}{1}
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

### Step 3. Calculate X

We use:

$$
X=A^{-1}B
$$

Substituting the matrices:

$$
X=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Multiplying the matrices:

$$
X=
\begin{pmatrix}
1\cdot3+(-2)\cdot2 & 1\cdot1+(-2)\cdot4 \\
0\cdot3+1\cdot2 & 0\cdot1+1\cdot4
\end{pmatrix}
$$

$$
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

### Step 4. Check the Result by Computing AX

We substitute the calculated matrix $X$ into the original equation:

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

Multiplying:

$$
AX=
\begin{pmatrix}
1\cdot(-1)+2\cdot2 & 1\cdot(-7)+2\cdot4 \\
0\cdot(-1)+1\cdot2 & 0\cdot(-7)+1\cdot4
\end{pmatrix}
$$

$$
AX=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

This is exactly equal to matrix $B$.

### Final Answer

$$
\boxed{
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
}
$$

### Conclusion

The inverse matrix $A^{-1}$ must be multiplied on the left side because $A$ is on the left side of $X$ in the equation $AX=B$.

The result is verified because $AX=B$.
