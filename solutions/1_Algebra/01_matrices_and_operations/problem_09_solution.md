# Exercise 9: Composing Transformations

## Question

Given the matrices:

$$
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},
\qquad
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

The matrix $S$ represents nonuniform scaling, while $R$ represents a $90^\circ$ counterclockwise rotation.

The given vector is:

$$
x=\begin{pmatrix}1\\2\end{pmatrix}
$$

Compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

### 1. Understand the Given Transformations

We are given three mathematical objects:

- Matrix $S$ performs nonuniform scaling. It doubles the horizontal coordinate and leaves the vertical coordinate unchanged.
- Matrix $R$ performs a $90^\circ$ counterclockwise rotation.
- Vector $x$ represents the initial point.

The matrices and vector are:

$$
S=\begin{pmatrix}2&0\\0&1\end{pmatrix}
$$

$$
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

$$
x=\begin{pmatrix}1\\2\end{pmatrix}
$$

Both matrices are $2\times2$, and the vector has two components. Therefore, all required multiplications are defined.

### 2. Calculate RSx

In matrix multiplication, the rightmost transformation is applied first.

Therefore, $RSx$ means that we first apply $S$ to $x$, and then apply $R$ to the resulting vector.

**Step 1: Apply the scaling transformation.**

$$
Sx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
$$

Using row-by-column multiplication:

First component:

$$
2\cdot1+0\cdot2=2
$$

Second component:

$$
0\cdot1+1\cdot2=2
$$

Therefore:

$$
Sx=\begin{pmatrix}2\\2\end{pmatrix}
$$

**Step 2: Apply the rotation transformation.**

Now we multiply the result by matrix $R$:

$$
RSx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}2\\2\end{pmatrix}
$$

First component:

$$
0\cdot2+(-1)\cdot2=-2
$$

Second component:

$$
1\cdot2+0\cdot2=2
$$

Thus:

$$
\boxed{RSx=\begin{pmatrix}-2\\2\end{pmatrix}}
$$

### 3. Calculate SRx

Now we reverse the order of the transformations.

For $SRx$, we first apply the rotation $R$, and then apply the scaling transformation $S$.

**Step 1: Apply the rotation transformation.**

$$
Rx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
$$

First component:

$$
0\cdot1+(-1)\cdot2=-2
$$

Second component:

$$
1\cdot1+0\cdot2=1
$$

Therefore:

$$
Rx=\begin{pmatrix}-2\\1\end{pmatrix}
$$

**Step 2: Apply the scaling transformation.**

Now multiply the result by matrix $S$:

$$
SRx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}-2\\1\end{pmatrix}
$$

First component:

$$
2\cdot(-2)+0\cdot1=-4
$$

Second component:

$$
0\cdot(-2)+1\cdot1=1
$$

Thus:

$$
\boxed{SRx=\begin{pmatrix}-4\\1\end{pmatrix}}
$$

### 4. Compare the Results

We obtained:

$$
RSx=\begin{pmatrix}-2\\2\end{pmatrix}
$$

and

$$
SRx=\begin{pmatrix}-4\\1\end{pmatrix}
$$

Comparing the two results:

$$
\begin{pmatrix}-2\\2\end{pmatrix}
\neq
\begin{pmatrix}-4\\1\end{pmatrix}
$$

Therefore:

$$
\boxed{RSx\neq SRx}
$$

This proves that changing the order of the transformations changes the final result.

### 5. Geometric Explanation

The difference can be explained geometrically.

**First case: Scaling followed by rotation (RSx).**

- The original vector is $(1,2)$.
- The scaling transformation doubles the horizontal coordinate.
- The vector becomes $(2,2)$.
- The rotation turns this vector $90^\circ$ counterclockwise.
- The final vector is $(-2,2)$.

**Second case: Rotation followed by scaling (SRx).**

- The original vector is $(1,2)$.
- The rotation turns the vector $90^\circ$ counterclockwise.
- The vector becomes $(-2,1)$.
- The scaling transformation doubles its horizontal coordinate.
- The final vector is $(-4,1)$.

The results are different because the scaling transformation affects the horizontal coordinate. Rotating the vector before scaling changes which coordinate is affected by the scaling operation.

### 6. Final Answer

The results are:

$$
\boxed{RSx=\begin{pmatrix}-2\\2\end{pmatrix}}
$$

$$
\boxed{SRx=\begin{pmatrix}-4\\1\end{pmatrix}}
$$

Since the two results are different:

$$
\boxed{RSx\neq SRx}
$$

**Conclusion:**

Matrix multiplication represents the composition of transformations. The order of transformations matters because matrix multiplication is generally not commutative.

In this example, applying nonuniform scaling before rotation produces a different result from applying rotation before nonuniform scaling. This demonstrates why the order of matrix transformations must be carefully considered.ifferent result from applying rotation before nonuniform scaling. This demonstrates why the order of matrix transformations must be carefully considered.
