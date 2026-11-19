# Exercise 7. Choosing a Method Deliberately

## Question

**Given:**

We consider three distinct linear system scenarios:

1. **Case 1:** A system with a triangular coefficient matrix:

$$2x - y = 3$$

$$4y = 8$$

2. **Case 2:** Three systems $Ax = b_i$ ($i = 1, 2, 3$) sharing the same invertible matrix $A$, where $A^{-1}$ is already known.
3. **Case 3:** One $3 \times 3$ system where $A^{-1}$ is not given and the goal is only to find a single solution vector.

**Required:**

1. For each situation, choose the method that best exploits its structure and justify the choice based on the **number of right-hand sides** and the **structure of the matrix**.
2. Carry out the chosen method **completely for Case 1**.
3. For **Cases 2 and 3**, describe the solution plan and indicate which parts of the computation are **reusable** or **unnecessary**.

> **Why this exercise:** Practices choosing a method based on the structure of the problem instead of solving another small system by two methods.

---

## Solution

### Step 1. Case 1 — Triangular Coefficient Matrix (Back-Substitution)

**Chosen Method & Justification:**

Use **back-substitution** directly. Because the coefficient matrix $\begin{bmatrix} 2 & -1 \\ 0 & 4 \end{bmatrix}$ is already upper triangular and there is only one right-hand side, no elimination or matrix inversion is required.

**Complete Solution for Case 1:**

$$2x - y = 3$$

$$4y = 8$$

1. **Solve for $y$ from the second equation:**

$$4y = 8 \implies y = \dfrac{8}{4} = 2$$

2. **Substitute $y = 2$ into the first equation to solve for $x$:**

$$2x - 2 = 3 \implies 2x = 5 \implies x = \dfrac{5}{2}$$

Thus, for Case 1:

$$(x,\ y) = \left(\dfrac{5}{2},\ 2\right)$$

---

### Step 2. Case 2 — Multiple Right-Hand Sides ($Ax = b_i$) With Known $A^{-1}$

**Chosen Method & Justification:**

Use direct matrix-vector multiplication:

$$x_i = A^{-1}b_i \qquad (i = 1, 2, 3)$$

Since there are three right-hand sides sharing the same invertible matrix $A$ and $A^{-1}$ is already known, multiplying $A^{-1}$ by each $b_i$ is much faster than performing elimination three separate times.

- **Plan:** Compute $x_1 = A^{-1}b_1$, $x_2 = A^{-1}b_2$, and $x_3 = A^{-1}b_3$.
- **Reusable:** The known inverse matrix **$A^{-1}$** is reused across all three right-hand sides $b_1, b_2, b_3$.
- **Unnecessary:** Computing $\det(A)$ or finding $A^{-1}$ from scratch is unnecessary.

---

### Step 3. Case 3 — One $3 \times 3$ System, Unknown $A^{-1}$, Single Solution Vector

**Chosen Method & Justification:**

Use **Gaussian elimination with back-substitution** on the augmented matrix $[A \mid b]$. Because $A$ is a general $3 \times 3$ matrix without triangular structure and there is only one right-hand side, reducing $[A \mid b]$ directly requires fewer operations than inverting $A$.

- **Plan:** Form $[A \mid b]$, reduce it to row echelon form using row operations, and find $x$ via back-substitution.
- **Reusable:** The **row operations** applied to $A$ are reused simultaneously on the right-hand side column $b$ during elimination.
- **Unnecessary:** Explicitly **computing $A^{-1}$** and multiplying $A^{-1}b$ are unnecessary since only one solution vector is needed.

---

### Final Answer

- **Case 1 (Triangular system, 1 RHS):** Use **back-substitution** directly:

$$(x,\ y) = \left(\dfrac{5}{2},\ 2\right)$$

- **Case 2 (3 systems $Ax = b_i$, same invertible $A$, $A^{-1}$ known):** Compute **$x_i = A^{-1}b_i$**; **$A^{-1}$** is reusable, computing $A^{-1}$ is unnecessary.
- **Case 3 (1 system of size $3 \times 3$, $A^{-1}$ unknown, 1 solution):** Use **Gaussian elimination + back-substitution** on $[A \mid b]$; row operations on $b$ are reusable, finding $A^{-1}$ is unnecessary.
