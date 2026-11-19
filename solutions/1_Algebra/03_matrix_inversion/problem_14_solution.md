# Exercise 14. A Matrix That Is Its Own Inverse

## Question

**Given:**

Assume that a square matrix $A$ satisfies the condition:

$$\large A^2 = I$$

where $I$ is the identity matrix of the same size as $A$.

**Required:**

1. Show that $A^{-1} = A$.
2. Give an example of a $2 \times 2$ matrix different from $I$ and $-I$ that satisfies $A^2 = I$.
3. Verify the chosen $2 \times 2$ example by matrix multiplication.

> **Why this exercise:** Requires using the definition of the inverse in a short argument and constructing an example independently, without introducing a new topic.

---

## Solution

### Step 1. Show That $A^{-1} = A$

By the definition of an inverse matrix, an invertible matrix $A$ has an inverse $A^{-1}$ if and only if:

$$\large A A^{-1} = I \qquad \text{and} \qquad A^{-1} A = I$$

We are given that:

$$\large A^2 = I$$

Rewriting $A^2$ as a product of $A$ with itself gives:

$$\large A \cdot A = I$$

Comparing $A \cdot A = I$ with the defining property $A \cdot A^{-1} = I$ (and by uniqueness of the inverse matrix), we conclude that:

$$\large A^{-1} = A$$

---

### Step 2. Construct a $2 \times 2$ Example Different from $I$ and $-I$

Consider the $2 \times 2$ reflection matrix:

$$\large A = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$$

Clearly, $A \neq I$ and $A \neq -I$, since:

$$\large I = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} \qquad \text{and} \qquad -I = \begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix}$$

---

### Step 3. Verify the Example by Multiplication

We compute $A^2 = A \cdot A$:

$$\large A^2 = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$$

Multiplying entry by entry:

$$\large A^2 = \begin{bmatrix} 0 \cdot 0 + 1 \cdot 1 & 0 \cdot 1 + 1 \cdot 0 \\ 1 \cdot 0 + 0 \cdot 1 & 1 \cdot 1 + 0 \cdot 0 \end{bmatrix}$$

Simplifying each entry gives:

$$\large A^2 = \begin{bmatrix} 0 + 1 & 0 + 0 \\ 0 + 0 & 0 + 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$$

Since $A^2 = I$, our matrix $A = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$ is indeed its own inverse ($A^{-1} = A$).

---

### Final Answer

1. **Proof:** Since $A^2 = A \cdot A = I$, by the definition and uniqueness of the matrix inverse, we have:

$$\large A^{-1} = A$$

2. **Example $2 \times 2$ matrix ($\neq I, -I$):**

$$\large A = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$$

3. **Verification:**

$$\large A^2 = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$$
