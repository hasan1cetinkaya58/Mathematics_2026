Exercise 2. Determinant of a 3×3 Matrix

Given:

A=\begin{pmatrix}
1&2&-1\\
0&3&4\\
2&1&5
\end{pmatrix}

Using Sarrus’ rule:

\det(A)=
1(3)(5)+2(4)(2)+(-1)(0)(1)

- [(-1)(3)(2)+2(0)(5)+1(4)(1)]

=15+16-(-6+4)

=31-(-2)

\boxed{\det(A)=33}

Check:

Perform the row operation:

R_3\leftarrow R_3-2R_1

The determinant does not change.

\begin{pmatrix}
1&2&-1\\
0&3&4\\
0&-3&7
\end{pmatrix}

Expanding along the first column:

\det(A)=1(3\cdot7-4(-3))

=21+12=\boxed{33}

Both methods give the same result.
