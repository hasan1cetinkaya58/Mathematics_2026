
# Exercise 13: A Recurrence Written in Matrix Form

## Question

Given the matrix:

$$
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

Compute F², F³, F⁴, and F⁵. Compare the results with the Fibonacci sequence and explain how matrix multiplication performs one recurrence step.

Also compute F(a,b)^T = (a+b,a)^T and explain how this multiplication advances the Fibonacci recurrence.

## Solution

### 1. Identify the Given Matrix

We are given:

$$
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

### 2. Calculate the Second Power

$$
F^2=F\cdot F
$$

$$
F^2=
\begin{pmatrix}1&1\\1&0\end{pmatrix}
\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

Calculating each entry:

- First row, first column: 1·1 + 1·1 = 2
- First row, second column: 1·1 + 1·0 = 1
- Second row, first column: 1·1 + 0·1 = 1
- Second row, second column: 1·1 + 0·0 = 1

Therefore:

$$
F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix}
$$

### 3. Calculate the Third Power

$$
F^3=F^2\cdot F
$$

$$
F^3=
\begin{pmatrix}2&1\\1&1\end{pmatrix}
\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

Calculating each entry:

- First row, first column: 2·1 + 1·1 = 3
- First row, second column: 2·1 + 1·0 = 2
- Second row, first column: 1·1 + 1·1 = 2
- Second row, second column: 1·1 + 1·0 = 1

Therefore:

$$
F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix}
$$

### 4. Calculate the Fourth Power

$$
F^4=F^3\cdot F
$$

$$
F^4=
\begin{pmatrix}3&2\\2&1\end{pmatrix}
\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

Calculating each entry:

- First row, first column: 3·1 + 2·1 = 5
- First row, second column: 3·1 + 2·0 = 3
- Second row, first column: 2·1 + 1·1 = 3
- Second row, second column: 2·1 + 1·0 = 2

Therefore:

$$
F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix}
$$

### 5. Calculate the Fifth Power

$$
F^5=F^4\cdot F
$$

$$
F^5=
\begin{pmatrix}5&3\\3&2\end{pmatrix}
\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

Calculating each entry:

- First row, first column: 5·1 + 3·1 = 8
- First row, second column: 5·1 + 3·0 = 5
- Second row, first column: 3·1 + 2·1 = 5
- Second row, second column: 3·1 + 2·0 = 3

Therefore:

$$
F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}
$$

### 6. Compare with the Fibonacci Sequence

The Fibonacci sequence is:

0, 1, 1, 2, 3, 5, 8, 13, ...

Our results are:

- F² = [[2, 1], [1, 1]]
- F³ = [[3, 2], [2, 1]]
- F⁴ = [[5, 3], [3, 2]]
- F⁵ = [[8, 5], [5, 3]]

We observe that the entries are consecutive Fibonacci numbers.

The general formula is:

$$
F^n=
\begin{pmatrix}
Fib_{n+1}&Fib_n\\
Fib_n&Fib_{n-1}
\end{pmatrix}
$$

where Fib₀ = 0 and Fib₁ = 1.

### 7. Calculate the Matrix Product F(a,b)

Let the column vector contain two consecutive terms:

( a )
( b )

Multiplying by matrix F:

F × (a, b)ᵀ = (a + b, a)ᵀ

Calculating the first entry:

1 × a + 1 × b = a + b

Calculating the second entry:

1 × a + 0 × b = a

Therefore, the resulting column vector is:

( a + b )
( a     )

### 8. Explain the Recurrence Step

This multiplication performs exactly one Fibonacci recurrence step.

- The first new entry is the sum of the previous two entries.
- The second new entry keeps the previous first entry.
- The resulting vector is ready for the next step.

For example:

(3, 2) → (5, 3)

Since 3 + 2 = 5, the next pair becomes (5, 3).

### 9. Final Conclusion

The calculations demonstrate that powers of matrix F generate consecutive Fibonacci numbers.

The general relationship is:

$$
F^n=
\begin{pmatrix}
Fib_{n+1}&Fib_n\\
Fib_n&Fib_{n-1}
\end{pmatrix}
$$

Furthermore, multiplying F by a vector containing two consecutive terms produces their sum and preserves the previous first term.

Thus, matrix multiplication provides a systematic way to represent and perform the Fibonacci recurrence.
