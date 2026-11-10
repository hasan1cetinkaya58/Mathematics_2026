
# Exercise 12: Formula for a Matrix Power

## Question

Given the matrix:

$$
A=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Compute \(A^2\), \(A^3\), and \(A^4\). Formulate a conjecture for \(A^n\), and prove the formula using mathematical induction.

## Solution

### 1. Calculate the Second Power \(A^2\)

By definition:

$$
A^2=A\cdot A
$$

Substituting the matrix:

$$
A^2=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
1\cdot1+1\cdot0=1
$$

First row, second column:

$$
1\cdot1+1\cdot1=2
$$

Second row, first column:

$$
0\cdot1+1\cdot0=0
$$

Second row, second column:

$$
0\cdot1+1\cdot1=1
$$

Therefore:

$$
A^2=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

### 2. Calculate the Third Power \(A^3\)

We multiply \(A^2\) by \(A\):

$$
A^3=A^2\cdot A
$$

$$
A^3=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
1\cdot1+2\cdot0=1
$$

First row, second column:

$$
1\cdot1+2\cdot1=3
$$

Second row, first column:

$$
0\cdot1+1\cdot0=0
$$

Second row, second column:

$$
0\cdot1+1\cdot1=1
$$

Therefore:

$$
A^3=
\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
$$

### 3. Calculate the Fourth Power \(A^4\)

We multiply \(A^3\) by \(A\):

$$
A^4=A^3\cdot A
$$

$$
A^4=
\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
1\cdot1+3\cdot0=1
$$

First row, second column:

$$
1\cdot1+3\cdot1=4
$$

Second row, first column:

$$
0\cdot1+1\cdot0=0
$$

Second row, second column:

$$
0\cdot1+1\cdot1=1
$$

Therefore:

$$
A^4=
\begin{pmatrix}
1 & 4\\
0 & 1
\end{pmatrix}
$$

### 4. Identify the Pattern and Formulate a Conjecture

We have calculated:

$$
A^2=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
$$

$$
A^4=
\begin{pmatrix}
1 & 4\\
0 & 1
\end{pmatrix}
$$

We can observe the following pattern:

- The diagonal entries always remain equal to 1.
- The bottom-left entry always remains equal to 0.
- The top-right entry increases by 1 with each multiplication by A.

Therefore, we conjecture that for every positive integer n:

$$
\boxed{
A^n=
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
}
$$

### 5. Prove the Formula Using Mathematical Induction

We will prove that:

$$
A^n=
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
$$

for every positive integer n.

**Base Case:**

For \(n=1\), the original matrix is:

$$
A^1=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Using our proposed formula:

$$
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Both expressions are equal. Therefore, the formula is true for \(n=1\).

**Inductive Hypothesis:**

Assume that the formula is true for some positive integer n.

Thus, we assume:

$$
A^n=
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
$$

**Inductive Step:**

We must show that the formula is also true for \(n+1\).

By the definition of matrix powers:

$$
A^{n+1}=A^n\cdot A
$$

Substituting the inductive hypothesis and the original matrix:

$$
A^{n+1}=
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Multiplying the matrices:

First row, first column:

$$
1\cdot1+n\cdot0=1
$$

First row, second column:

$$
1\cdot1+n\cdot1=1+n
$$

Second row, first column:

$$
0\cdot1+1\cdot0=0
$$

Second row, second column:

$$
0\cdot1+1\cdot1=1
$$

Therefore:

$$
A^{n+1}=
\begin{pmatrix}
1 & n+1\\
0 & 1
\end{pmatrix}
$$

This is exactly the proposed formula with n replaced by n+1.

Therefore, the inductive step is complete.

### 6. Final Conclusion

We have verified the formula for the base case and proved that if it is true for n, it must also be true for n+1.

By mathematical induction, the formula holds for every positive integer n:

$$
\boxed{
A^n=
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
}
$$

The pattern shows that each multiplication by A increases the top-right entry by 1, while all other entries remain unchanged.

This exercise demonstrates how a pattern observed through several matrix calculations can be generalized and rigorously proven using mathematical induction.
