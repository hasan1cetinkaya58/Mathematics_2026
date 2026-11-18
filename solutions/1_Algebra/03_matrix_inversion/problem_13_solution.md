# Exercise 13. Undoing a Composite Transformation

## Question

**Given:**

The matrices describing nonuniform scaling and shear are:

$$\large S = \begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix}, \qquad H = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix}$$

Let $T = HS$.

**Required:**

1. Find $T^{-1}$ in two ways:
   - **Method 1:** First compute $T$, then compute its inverse $T^{-1}$.
   - **Method 2:** Use the inverse of a product property $(HS)^{-1} = S^{-1}H^{-1}$.
2. Compare the results from both methods.
3. Compute $H^{-1}S^{-1}$ and verify that multiplying the inverses in the incorrect order gives a different matrix.
4. Explain the rule: *"When undoing a composition of operations, we undo them from the end."*

> **Why this exercise:** Reinforces the inverse of a product in a less direct configuration.

---

## Solution

### Step 1. Method 1 — Compute $T$ First, Then Find $T^{-1}$First, we compute the composite transformation matrix $T = HS$:

$$\large T = HS = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix}$$

Performing the matrix multiplication entry by entry:

$$\large T = \begin{bmatrix} 1 \cdot 2 + 1 \cdot 0 & 1 \cdot 0 + 1 \cdot 1 \\ 0 \cdot 2 + 1 \cdot 0 & 0 \cdot 0 + 1 \cdot 1 \end{bmatrix}$$

Simplifying gives:

$$\large T = \begin{bmatrix} 2 & 1 \\ 0 & 1 \end{bmatrix}$$

Next, we find the inverse of $T = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ using the general $2 \times 2$ inverse formula:

$$\large T^{-1} = \dfrac{1}{ad - bc} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

We first calculate the determinant of $T$:

$$\large \det(T) = (2)(1) - (1)(0) = 2 \neq 0$$

Since $\det(T) \neq 0$, $T$ is invertible. Substituting the entries into the inverse formula gives:

$$\large T^{-1} = \dfrac{1}{2} \begin{bmatrix} 1 & -1 \\ 0 & 2 \end{bmatrix}$$

Multiplying each entry by the scalar $\dfrac{1}{2}$:

$$\large T^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix}$$

---### Step 2. Method 2 — Use the Product Property $(HS)^{-1} = S^{-1}H^{-1}$First, we compute the individual inverses $S^{-1}$ and $H^{-1}$ separately.

For $S = \begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix}$, the determinant is $\det(S) = (2)(1) - (0)(0) = 2$:

$$\large S^{-1} = \dfrac{1}{2} \begin{bmatrix} 1 & 0 \\ 0 & 2 \end{bmatrix} = \begin{bmatrix} \dfrac{1}{2} & 0 \\ 0 & 1 \end{bmatrix}$$

For $H = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix}$, the determinant is $\det(H) = (1)(1) - (1)(0) = 1$:

$$\large H^{-1} = \dfrac{1}{1} \begin{bmatrix} 1 & -1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} 1 & -1 \\ 0 & 1 \end{bmatrix}$$

Now, we multiply the individual inverses in reverse order ($S^{-1}H^{-1}$):

$$\large S^{-1}H^{-1} = \begin{bmatrix} \dfrac{1}{2} & 0 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & -1 \\ 0 & 1 \end{bmatrix}$$

Performing the matrix multiplication step by step:

$$\large S^{-1}H^{-1} = \begin{bmatrix} \dfrac{1}{2} \cdot 1 + 0 \cdot 0 & \dfrac{1}{2} \cdot (-1) + 0 \cdot 1 \\ 0 \cdot 1 + 1 \cdot 0 & 0 \cdot (-1) + 1 \cdot 1 \end{bmatrix}$$

Simplifying each entry yields:

$$\large S^{-1}H^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix}$$

---### Step 3. Compare the Two Results

Comparing the inverse matrices obtained in Step 1 and Step 2:

$$\large T^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix} \qquad \text{and} \qquad S^{-1}H^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix}$$

Both methods yield the exact same inverse matrix, confirming the product rule $(HS)^{-1} = S^{-1}H^{-1}$.

---

### Step 4. Compute $H^{-1}S^{-1}$ (Incorrect Order) and Verify

Now, we multiply the inverses in the original order $H^{-1}S^{-1}$:

$$\large H^{-1}S^{-1} = \begin{bmatrix} 1 & -1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} \dfrac{1}{2} & 0 \\ 0 & 1 \end{bmatrix}$$

Performing the matrix multiplication:

$$\large H^{-1}S^{-1} = \begin{bmatrix} 1 \cdot \dfrac{1}{2} + (-1) \cdot 0 & 1 \cdot 0 + (-1) \cdot 1 \\ 0 \cdot \dfrac{1}{2} + 1 \cdot 0 & 0 \cdot 0 + 1 \cdot 1 \end{bmatrix}$$

Simpl
