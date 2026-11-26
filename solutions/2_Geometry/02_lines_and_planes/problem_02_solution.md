# Exercise 2. A Line in Space

## Question

**Given:**

The line $L$ in $\mathbb{R}^3$ defined by:

$$L: (x, y, z) = (2, -1, 3) + t(1, 2, -2), \qquad t \in \mathbb{R}$$

**Required:**

1. State a point on the line and its direction vector.
2. Check whether $P = (4, 3, -1)$ lies on $L$.
3. Find the point corresponding to $t = -1$.

> **Why this exercise:** Reinforces the interpretation of parametric form as "point + direction."

---

## Solution

### Step 1. Identify a Point and Direction Vector

Comparing $L: (x, y, z) = (2, -1, 3) + t(1, 2, -2)$ with the standard form $r(t) = P_0 + t d$:

- **Point on the line ($t = 0$):** $P_0 = (2, -1, 3)$
- **Direction vector:** $d = (1, 2, -2)$

---

### Step 2. Check Whether $P = (4, 3, -1)$ Lies on $L$

Point $P = (4, 3, -1)$ lies on $L$ if there exists a single scalar $t \in \mathbb{R}$ satisfying all three coordinate equations simultaneously:

$$2 + t = 4 \implies t = 2$$

$$-1 + 2t = 3 \implies 2t = 4 \implies t = 2$$

$$3 - 2t = -1 \implies -2t = -4 \implies t = 2$$

Since all three equations yield the same parameter value $t = 2$, the point $P = (4, 3, -1)$ **lies on $L$**.

---

### Step 3. Find the Point Corresponding to $t = -1$

Substitute $t = -1$ into the parametric equation of $L$:

$$(x, y, z) = (2, -1, 3) + (-1)(1, 2, -2) = (2 - 1,\ -1 - 2,\ 3 + 2) = (1, -3, 5)$$

---

### Final Answer

- **Point on the line:** $P_0 = (2, -1, 3)$
- **Direction vector:** $d = (1, 2, -2)$
- **Does $P = (4, 3, -1)$ lie on $L$?** Yes, for $t = 2$.
- **Point at $t = -1$:** $(1, -3, 5)$
