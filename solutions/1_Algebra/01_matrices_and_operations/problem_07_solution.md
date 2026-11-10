
# Exercise 7: Identity Matrix, Zero Matrix, and Powers

## Question

For the matrix

$$
A=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
$$

Compute:

$$
AI,\quad IA,\quad A+0,\quad A^2,\quad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern observed in successive powers of $A$.

## Solution

### 1. Identify the Given Matrix

The given matrix is:

$$
A=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
$$

It is a square matrix with dimensions $2\times2$.

To perform the required operations, we first define the identity matrix and the zero matrix of the same dimensions.

The identity matrix is:

$$
I=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
$$

The zero matrix is:

$$
0=
\begin{pmatrix}
0&0\\
0&0
\end{pmatrix}
$$

### 2. Calculate AI

The identity matrix does not change a matrix when multiplied by it.

We calculate:

$$
AI=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
$$

Using row-by-column multiplication:

First row, first column:

$$
2\cdot1+1\cdot0=2
$$

First row, second column:

$$
2\cdot0+1\cdot1=1
$$

Second row, first column:

$$
0\cdot1+2\cdot0=0
$$

Second row, second column:

$$
0\cdot0+2\cdot1=2
$$

Therefore:

$$
\boxed{
AI=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}=A
}
$$

### 3. Calculate IA

Now we multiply the identity matrix by $A$ in the reverse order.

$$
IA=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
$$

Using row-by-column multiplication:

First row, first column:

$$
1\cdot2+0\cdot0=2
$$

First row, second column:

$$
1\cdot1+0\cdot2=1
$$

Second row, first column:

$$
0\cdot2+1\cdot0=0
$$

Second row, second column:

$$
0\cdot1+1\cdot2=2
$$

Therefore:

$$
\boxed{
IA=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}=A
}
$$

This confirms that multiplying a matrix by the identity matrix on either side leaves the original matrix unchanged.

### 4. Calculate A + 0

The zero matrix contains only zeros.

When we add two matrices, we add their corresponding entries.

$$
A+0=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
+
\begin{pmatrix}
0&0\\
0&0
\end{pmatrix}
$$

Adding the corresponding entries:

$$
A+0=
\begin{pmatrix}
2+0&1+0\\
0+0&2+0
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A+0=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}=A
}
$$

The zero matrix does not change a matrix when added to it.

### 5. Calculate A²

The second power of a matrix means multiplying the matrix by itself.

$$
A^2=A\cdot A
$$

Substituting the given matrix:

$$
A^2=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
$$

We calculate each entry separately.

First row, first column:

$$
2\cdot2+1\cdot0=4
$$

First row, second column:

$$
2\cdot1+1\cdot2=2+2=4
$$

Second row, first column:

$$
0\cdot2+2\cdot0=0
$$

Second row, second column:

$$
0\cdot1+2\cdot2=4
$$

Therefore:

$$
\boxed{
A^2=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}
}
$$

### 6. Calculate A³

The third power means multiplying $A^2$ by the original matrix $A$.

$$
A^3=A^2\cdot A
$$

We substitute the matrices:

$$
A^3=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
$$

Now calculate each entry.

First row, first column:

$$
4\cdot2+4\cdot0=8
$$

First row, second column:

$$
4\cdot1+4\cdot2=4+8=12
$$

Second row, first column:

$$
0\cdot2+4\cdot0=0
$$

Second row, second column:

$$
0\cdot1+4\cdot2=8
$$

Therefore:

$$
\boxed{
A^3=
\begin{pmatrix}
8&12\\
0&8
\end{pmatrix}
}
$$

### 7. Explain the Roles of the Identity Matrix and the Zero Matrix

The identity matrix $I$ is the multiplicative identity.

This means that multiplying a matrix by the identity matrix does not change the original matrix.

For the given matrix:

$$
AI=IA=A
$$

The zero matrix $0$ is the additive identity.

This means that adding the zero matrix to another matrix does not change that matrix.

For the given matrix:

$$
A+0=A
$$

Therefore, the identity matrix plays the role of the neutral element in matrix multiplication, while the zero matrix plays the role of the neutral element in matrix addition.

### 8. Observe the Pattern in Successive Powers of A

We have calculated the first three powers:

$$
A=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}
$$

$$
A^2=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}
8&12\\
0&8
\end{pmatrix}
$$

By comparing these matrices, we can observe the following pattern:

- The diagonal entries double with each successive power.
- The bottom-left entry remains zero.
- The top-right entry changes from 1 to 4 and then to 12.

The diagonal entries follow the sequence:

$$
2,\quad4,\quad8
$$

The top-right entries follow the sequence:

$$
1,\quad4,\quad12
$$

More generally, for a positive integer $n$, the pattern is:

$$
A^n=
\begin{pmatrix}
2^n&n\cdot2^{n-1}\\
0&2^n
\end{pmatrix}
$$

This formula describes the pattern observed in successive powers of the given matrix.

## Final Answer

The identity matrix products are:

$$
\boxed{AI=IA=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}}
$$

The addition with the zero matrix is:

$$
\boxed{A+0=
\begin{pmatrix}
2&1\\
0&2
\end{pmatrix}}
$$

The second power is:

$$
\boxed{A^2=
\begin{pmatrix}
4&4\\
0&4
\end{pmatrix}}
$$

The third power is:

$$
\boxed{A^3=
\begin{pmatrix}
8&12\\
0&8
\end{pmatrix}}
$$

**Conclusion:**

The identity matrix leaves a matrix unchanged under multiplication, while the zero matrix leaves a matrix unchanged under addition.

The successive powers of $A$ show a regular pattern: the diagonal entries double, the bottom-left entry remains zero, and the top-right entry follows the sequence $1,4,12$.

This demonstrates how identity matrices, zero matrices, and matrix powers behave in matrix algebra.

