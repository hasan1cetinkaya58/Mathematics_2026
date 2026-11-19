# Exercise 1. From a System to a Matrix

## Question

**Given:**

Consider the following system of three linear equations in three unknowns:

$$2x - y + z = 4$$

$$x + 3y - 2z = 1$$

$$3x + y + z = 7$$

**Required:**

1. Write the system in the matrix form $Ax = b$.
2. Identify the coefficient matrix $A$, the vector of unknowns $x$, and the right-hand side vector $b$.
3. Explain how each row of the matrix corresponds to one equation.

> **Why this exercise:** Teaches how to move between a system of equations and matrix notation.

---

## Solution

### Step 1. Write the System in the Form $Ax = b$

To express the linear system in the matrix equation form $Ax = b$, we align the variables $x$, $y$, and $z$ vertically across all three equations:

$$2x - 1y + 1z = 4$$

$$1x + 3y - 2z = 1$$

$$3x + 1y + 1z = 7$$

Writing this in the compact matrix form $Ax = b$ gives:

$$\begin{bmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 4 \\ 1 \\ 7 \end{bmatrix}$$

---

### Step 2. Identify $A$, $x$, and $b$

From the matrix equation above, we identify the three components:

1. **Coefficient matrix ($A$):**

$$A = \begin{bmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \end{bmatrix}$$

2. **Vector of unknowns ($x$):**

$$x = \begin{bmatrix} x \\ y \\ z \end{bmatrix}$$

3. **Right-hand side vector ($b$):**

$$b = \begin{bmatrix} 4 \\ 1 \\ 7 \end{bmatrix}$$

---

### Step 3. Explain How Each Row Corresponds to One Equation

When multiplying the $3 \times 3$ coefficient matrix $A$ by the $3 \times 1$ column vector of unknowns $x$, each entry of the resulting $3 \times 1$ product $Ax$ is obtained as the dot product of a row of $A$ with the column vector $x$, which is then set equal to the corresponding entry in $b$:

- **Row 1 of $A$ and entry 1 of $b$:**

$$\begin{bmatrix} 2 & -1 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = 4 \implies 2x - y + z = 4 \quad \text{(First equation)}$$

- **Row 2 of $A$ and entry 2 of $b$:**

$$\begin{bmatrix} 1 & 3 & -2 \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = 1 \implies x + 3y - 2z = 1 \quad \text{(Second equation)}$$

- **Row 3 of $A$ and entry 3 of $b$:**

$$\begin{bmatrix} 3 & 1 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = 7 \implies 3x + y + z = 7 \quad \text{(Third equation)}$$

In general, the $i$-th row of $A$ stores the coefficients of the variables $(x, y, z)$ in the $i$-th equation, while the $i$-th entry of $b$ stores the constant on the right-hand side of that same equation.

---

### Final Answer

1. **Matrix form $Ax = b$:**

$$\begin{bmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 4 \\ 1 \\ 7 \end{bmatrix}$$

2. **Components:**

$$A = \begin{bmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \end{bmatrix}, \qquad x = \begin{bmatrix} x \\ y \\ z \end{bmatrix}, \qquad b = \begin{bmatrix} 4 \\ 1 \\ 7 \end{bmatrix}$$

3. **Row-to-equation correspondence:** Each row $i$ of $A$ contains the coefficients of $x, y, z$ from equation $i$, and multiplying row $i$ of $A$ by the unknown vector $x$ reproduces the left-hand side of equation $i$, which equals the $i$-th component of $b$.
