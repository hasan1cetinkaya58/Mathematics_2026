# Exercise 14. A System of Equations and the Determinant

## Question

Consider the system

$$
Ax=b,
$$

where

$$
A=\begin{pmatrix}
1&2\\
k&4
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$?

For the remaining value of $k$, give:
- An example of a right-hand side $b$ for which the system has infinitely many solutions.
- An example of a right-hand side $b$ for which the system has no solution.

## Solution

### Step 1. Calculate the Determinant

A square system has exactly one solution for every right-hand side $b$ if and only if its coefficient matrix is invertible.

A matrix is invertible if and only if its determinant is nonzero.

For the given matrix,

$$
A=\begin{pmatrix}
1&2\\
k&4
\end{pmatrix},
$$

the determinant is

$$
\det(A)=1\cdot4-2\cdot k.
$$

Therefore,

$$
\det(A)=4-2k.
$$

### Step 2. Find the Values of k for Which the Solution Is Unique

The matrix is invertible when its determinant is not zero.

Thus,

$$
4-2k\neq0.
$$

Solving this inequality gives

$$
k\neq2.
$$

Therefore, for every $k\neq2$, the system has exactly one solution for every right-hand side $b$.

### Step 3. Examine the Exceptional Case k = 2

When $k=2$, the coefficient matrix becomes

$$
A=\begin{pmatrix}
1&2\\
2&4
\end{pmatrix}.
$$

The corresponding system is

$$
\begin{cases}
x+2y=b_1,\\
2x+4y=b_2.
\end{cases}
$$

The second equation has a left-hand side that is twice the first equation.

Therefore, the two equations are dependent. The system may have infinitely many solutions or no solution, depending on the right-hand side $b$.

### Step 4. Give an Example with Infinitely Many Solutions

Choose

$$
b=\begin{pmatrix}
1\\
2
\end{pmatrix}.
$$

The system becomes

$$
\begin{cases}
x+2y=1,\\
2x+4y=2.
\end{cases}
$$

The second equation is exactly twice the first equation.

Thus, both equations describe the same line, and there are infinitely many solutions.

For example, all pairs satisfying

$$
x=1-2y
$$

are solutions.

### Step 5. Give an Example with No Solution

Now choose

$$
b=\begin{pmatrix}
1\\
3
\end{pmatrix}.
$$

The system becomes

$$
\begin{cases}
x+2y=1,\\
2x+4y=3.
\end{cases}
$$

Multiplying the first equation by $2$ gives

$$
2x+4y=2.
$$

However, the second equation requires

$$
2x+4y=3.
$$

These equations contradict each other. Therefore, the system has no solution.

### Step 6. Final Answer and Conclusion

The determinant is

$$
\det(A)=4-2k.
$$

Therefore:

- If $k\neq2$, the system has exactly one solution for every $b$.
- If $k=2$ and $b=(1,2)^T$, the system has infinitely many solutions.
- If $k=2$ and $b=(1,3)^T$, the system has no solution.

At the exceptional value $k=2$, the second row of the coefficient matrix is twice the first row. The rows are linearly dependent, which explains why the system does not have a unique solution for every right-hand side.
