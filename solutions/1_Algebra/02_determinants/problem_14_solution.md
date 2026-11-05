# Determinants – Exercise 14

## Exercise 14. A System of Equations and the Determinant

Given:

$$Ax=b,\qquad A=\begin{pmatrix}1&2\\k&4\end{pmatrix}$$

We need to find the values of k for which the system has exactly one
solution for every b.

### Step 1: Calculate the determinant.

$$\det(A)=1\cdot4-2\cdot k=4-2k$$

### Step 2: Apply the unique solution condition.

A system has exactly one solution for every right-hand side b if the
coefficient matrix is invertible.

$$\det(A)\neq0$$ $$4-2k\neq0$$ $$4\neq2k$$ $$\boxed{k\neq2}$$

### Step 3: Consider the exceptional case $k=2$.

Substitute $k=2$:

$$A=\begin{pmatrix}1&2\\2&4\end{pmatrix}$$

The system becomes:

$$x+2y=b_1$$ $$2x+4y=b_2$$

### Example 1: Infinitely many solutions

Choose:

$$b=\begin{pmatrix}1\\2\end{pmatrix}$$

The system becomes:

$$x+2y=1$$ $$2x+4y=2$$

The second equation is twice the first equation. Therefore, both
equations represent the same line.

$$x=1-2y$$

There are infinitely many possible values of x and y.

$$\boxed{\text{Infinitely many solutions}}$$

### Example 2: No solution

Choose:

$$b=\begin{pmatrix}1\\0\end{pmatrix}$$

The system becomes:

$$x+2y=1$$ $$2x+4y=0$$

Multiply the first equation by 2:

$$2x+4y=2$$

But the second equation says $2x+4y=0$. This gives the contradiction:

$$2=0$$

Therefore:

$$\boxed{\text{No solution}}$$


------------------------------------------------------------------------

