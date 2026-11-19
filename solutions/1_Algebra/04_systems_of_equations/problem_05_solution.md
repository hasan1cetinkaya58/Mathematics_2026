# Exercise 5. Row Echelon Form and Number of Solutions

## Question

**Given:**

Consider the linear system represented by the following augmented matrix in row echelon form:

$$\left[\begin{array}{ccc|c} 1 & 2 & -1 & 3 \\ 0 & 1 & 2 & 1 \\ 0 & 0 & 0 & 0 \end{array}\right]$$

**Required:**

1. Determine the number of solutions of the system.
2. Write the solutions in parametric form.
3. Explain how you know how many variables may be chosen freely.

> **Why this exercise:** Teaches how to read information about solutions directly from row echelon form.

---

## Solution

### Step 1. Analyze Consistency and Pivots in the Row Echelon Form

The given matrix is already in row echelon form:

$$\left[\begin{array}{ccc|c} 1 & 2 & -1 & 3 \\ 0 & 1 & 2 & 1 \\ 0 & 0 & 0 & 0 \end{array}\right]$$

- **Third row:** Corresponds to $0x_1 + 0x_2 + 0x_3 = 0$, which is always true ($0 = 0$) and imposes no contradiction. Therefore, the system is **consistent**.
- **Pivot columns:** The leading nonzero entries (pivots) are in **column 1** (row 1) and **column 2** (row 2). Thus, there are **$2$ pivot columns** (corresponding to the pivot variables $x_1$ and $x_2$).
- **Non-pivot columns:** **Column 3** has no pivot, so $x_3$ is a **free variable**.

---

### Step 2. Explain How Many Variables May Be Chosen Freely

For a consistent linear system with $n$ unknowns (columns in the coefficient matrix) and $r$ pivot columns (rank of the coefficient matrix):

$$\text{Number of free variables} = n - r$$

Here, there are $n = 3$ unknowns ($x_1, x_2, x_3$) and $r = 2$ pivot columns (columns $1$ and $2$). Therefore:

$$n - r = 3 - 2 = 1$$

Only **$1$ variable** may be chosen freely ($x_3$). Because the system is consistent and has at least one free variable, it has **infinitely many solutions**.

---

### Step 3. Write the Solutions in Parametric Form

Translate the nonzero rows of the row echelon matrix into equations:

$$x_1 + 2x_2 - x_3 = 3$$

$$x_2 + 2x_3 = 1$$

Let the free variable be $x_3 = t$, where $t \in \mathbb{R}$ is any real parameter.

1. **Express $x_2$ in terms of $t$ from the second equation:**

$$x_2 + 2t = 1 \implies x_2 = 1 - 2t$$

2. **Substitute $x_2 = 1 - 2t$ and $x_3 = t$ into the first equation to find $x_1$:**

$$x_1 + 2(1 - 2t) - t = 3$$

$$x_1 + 2 - 4t - t = 3$$

$$x_1 + 2 - 5t = 3 \implies x_1 = 1 + 5t$$

Thus, the general solution in parametric form is:

$$x_1 = 1 + 5t, \qquad x_2 = 1 - 2t, \qquad x_3 = t \qquad (t \in \mathbb{R})$$

Or in vector form:

$$\mathbf{x} = \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} 1 + 5t \\ 1 - 2t \\ t \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix} + t \begin{bmatrix} 5 \\ -2 \\ 1 \end{bmatrix}, \qquad t \in \mathbb{R}$$

---

### Final Answer

- **Number of solutions:** **Infinitely many solutions** (the system is consistent with $0 = 0$ in the third row and a free column).
- **Number of free variables:** **$1$ free variable** ($x_3$), since $n - r = 3 - 2 = 1$ (3 unknowns minus 2 pivot columns).
- **Parametric form:**

$$x_1 = 1 + 5t, \qquad x_2 = 1 - 2t, \qquad x_3 = t \qquad (t \in \mathbb{R})$$
