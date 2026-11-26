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

### Step 1. Method 1 — Compute $T$ First, Then Find $T^{-1}$

First, we compute the composite transformation matrix $T = HS$:

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

---

### Step 2. Method 2 — Use the Product Property $(HS)^{-1} = S^{-1}H^{-1}$

First, we compute the individual inverses $S^{-1}$ and $H^{-1}$ separately.

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

---

### Step 3. Compare the Two Results

Comparing the inverse matrices obtained in Step 1 and Step 2:

$$\large T^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix} \qquad \text{and} \qquad S^{-1}H^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix}$$

Both methods yield the exact same inverse matrix, confirming the product rule $(HS)^{-1} = S^{-1}H^{-1}$.

---

### Step 4. Compute $H^{-1}S^{-1}$ (Incorrect Order) and Verify

Now, we multiply the inverses in the original order $H^{-1}S^{-1}$:

$$\large H^{-1}S^{-1} = \begin{bmatrix} 1 & -1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} \dfrac{1}{2} & 0 \\ 0 & 1 \end{bmatrix}$$

Performing the matrix multiplication entry by entry:

$$\large H^{-1}S^{-1} = \begin{bmatrix} 1 \cdot \dfrac{1}{2} + (-1) \cdot 0 & 1 \cdot 0 + (-1) \cdot 1 \\ 0 \cdot \dfrac{1}{2} + 1 \cdot 0 & 0 \cdot 0 + 1 \cdot 1 \end{bmatrix}$$

Simplifying each entry gives:

$$\large H^{-1}S^{-1} = \begin{bmatrix} \dfrac{1}{2} & -1 \\ 0 & 1 \end{bmatrix}$$

Comparing $H^{-1}S^{-1}$ with the true inverse $T^{-1}$:

$$\large H^{-1}S^{-1} = \begin{bmatrix} \dfrac{1}{2} & -1 \\ 0 & 1 \end{bmatrix} \neq \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix} = T^{-1}$$

Multiplying the inverses in the wrong order produces a different top-right entry ($-1 \neq -\dfrac{1}{2}$), so $H^{-1}S^{-1} \neq (HS)^{-1}$.

---

### Step 5. Explanation of Undoing Operations from the End

In $T = HS$, when applied to a vector $x$, we compute $Tx = H(Sx)$:
1. First, the nonuniform scaling $S$ is applied to $x$.
2. Second, the shear $H$ is applied to the result $Sx$.

To return to the original vector $x$, we must undo the **last** operation first:
- First apply $H^{-1}$ to undo the shear: $H^{-1}(HSx) = (H^{-1}H)Sx = ISx = Sx$.
- Second apply $S^{-1}$ to undo the scaling: $S^{-1}(Sx) = (S^{-1}S)x = Ix = x$.

Combining both steps gives $S^{-1}H^{-1}(HS) = I$, which explains why $(HS)^{-1} = S^{-1}H^{-1}$: a sequence of operations is undone in reverse order, starting from the end.

---

### Final Answer

- **Inverse matrix $T^{-1}$ (both methods):**

$$\large T^{-1} = S^{-1}H^{-1} = \begin{bmatrix} \dfrac{1}{2} & -\dfrac{1}{2} \\ 0 & 1 \end{bmatrix}$$

- **Incorrect order product:**

$$\large H^{-1}S^{-1} = \begin{bmatrix} \dfrac{1}{2} & -1 \\ 0 & 1 \end{bmatrix} \neq T^{-1}$$

- **Rule summary:** Because $HS$ applies $S$ first and $H$ second, reversing the transformation requires undoing $H$ first via $H^{-1}$ and then undoing $S$ via $S^{-1}$, yielding $(HS)^{-1} = S^{-1}H^{-1}$.
