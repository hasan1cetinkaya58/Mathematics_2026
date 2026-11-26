# Exercise 8: Linear Combination and Checking the Result

## Question

Given the vectors:

- $w = (5, 1)$
- $u = (1, 1)$
- $v = (2, -1)$

Check whether $w$ can be written as:

$$w = au + bv$$

If so:

1. Find the values of $a$ and $b$.
2. Reconstruct $w$ using these coefficients.
3. Explain the geometric meaning of the existence of such coefficients.

---

## Solution

### 1. Finding the Coefficients $a$ and $b$

Substitute the given vectors into $w = au + bv$:

$$(5, 1) = a(1, 1) + b(2, -1) = (a + 2b,\ a - b)$$

Equating corresponding components gives the linear system:

$$a + 2b = 5$$

$$a - b = 1$$

Subtract the second equation from the first:

$$(a + 2b) - (a - b) = 5 - 1 \implies 3b = 4 \implies b = \frac{4}{3}$$

Substitute $b = \frac{4}{3}$ into $a - b = 1$:

$$a - \frac{4}{3} = 1 \implies a = 1 + \frac{4}{3} = \frac{7}{3}$$

Thus, the coefficients are $a = \frac{7}{3}$ and $b = \frac{4}{3}$.

### 2. Reconstructing the Original Vector

Substitute $a = \frac{7}{3}$ and $b = \frac{4}{3}$ into $w = au + bv$:

$$w = \frac{7}{3}(1, 1) + \frac{4}{3}(2, -1) = \left(\frac{7}{3}, \frac{7}{3}\right) + \left(\frac{8}{3}, -\frac{4}{3}\right) = \left(\frac{15}{3}, \frac{3}{3}\right) = (5, 1)$$

This matches the original vector $w = (5, 1)$, confirming the result.

### 3. Geometric Interpretation

Geometrically, $w = \frac{7}{3}u + \frac{4}{3}v$ means that $w$ is reached by scaling $u$ by a factor of $\frac{7}{3}$, scaling $v$ by a factor of $\frac{4}{3}$, and adding the two scaled vectors via the parallelogram rule.

Because $u = (1, 1)$ and $v = (2, -1)$ are not scalar multiples of one another, they point in two independent directions and span the entire plane $\mathbb{R}^2$. Consequently, every vector in $\mathbb{R}^2$—including $w = (5, 1)$—can be uniquely written as a linear combination of $u$ and $v$.

---

## Final Results

- **Coefficients:** $a = \frac{7}{3}$ and $b = \frac{4}{3}$
- **Linear combination:** $w = \frac{7}{3}u + \frac{4}{3}v$
- **Verification:** $\frac{7}{3}(1,1) + \frac{4}{3}(2,-1) = (5,1)$
- **Conclusion:** Yes, $w$ can be uniquely expressed as a linear combination of $u$ and $v$ because $u$ and $v$ are linearly independent and span $\mathbb{R}^2$.
