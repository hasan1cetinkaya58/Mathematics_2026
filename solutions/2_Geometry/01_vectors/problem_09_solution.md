# Exercise 9: Cross Product as a Perpendicular Direction

## Question

Given the vectors:

$$u = (1, 2, 0) \qquad \text{and} \qquad v = (0, 1, 3)$$

1. Compute $u \times v$.
2. Use dot products to check perpendicularity to both vectors.
3. Compute $v \times u$.
4. Compare the results.

---

## Solution

### 1. Computing the Cross Product $u \times v$

Using the cross product formula for $u = (u_1, u_2, u_3)$ and $v = (v_1, v_2, v_3)$:

$$u \times v = (u_2v_3 - u_3v_2,\ u_3v_1 - u_1v_3,\ u_1v_2 - u_2v_1)$$

Substituting $u = (1, 2, 0)$ and $v = (0, 1, 3)$:

$$u \times v = (2 \cdot 3 - 0 \cdot 1,\ 0 \cdot 0 - 1 \cdot 3,\ 1 \cdot 1 - 2 \cdot 0) = (6, -3, 1)$$

### 2. Checking Perpendicularity Using Dot Products

A vector is perpendicular to another if their dot product is zero.

- **Check against $u = (1, 2, 0)$:**

$$(u \times v) \cdot u = 6 \cdot 1 + (-3) \cdot 2 + 1 \cdot 0 = 6 - 6 + 0 = 0$$

- **Check against $v = (0, 1, 3)$:**

$$(u \times v) \cdot v = 6 \cdot 0 + (-3) \cdot 1 + 1 \cdot 3 = 0 - 3 + 3 = 0$$

Both dot products equal zero, confirming that $u \times v$ is perpendicular to both $u$ and $v$.

### 3. Computing the Cross Product $v \times u$

Reversing the order of the vectors:

$$v \times u = (v_2u_3 - v_3u_2,\ v_3u_1 - v_1u_3,\ v_1u_2 - v_2u_1)$$

Substituting the components:

$$v \times u = (1 \cdot 0 - 3 \cdot 2,\ 3 \cdot 1 - 0 \cdot 0,\ 0 \cdot 2 - 1 \cdot 1) = (-6, 3, -1)$$

### 4. Comparing the Results

Comparing $u \times v = (6, -3, 1)$ and $v \times u = (-6, 3, -1)$, every component has the opposite sign:

$$v \times u = -(u \times v)$$

This demonstrates that the cross product is **anti-commutative**: reversing the order of the vectors preserves the magnitude ($\|v \times u\| = \|u \times v\| = \sqrt{46}$) and perpendicularity to the plane spanned by $u$ and $v$, but reverses the orientation (points in the opposite direction).

---

## Final Results

- **Cross product $u \times v$:** $(6, -3, 1)$
- **Perpendicularity checks:** $(u \times v) \cdot u = 0$ and $(u \times v) \cdot v = 0$
- **Reversed cross product $v \times u$:** $(-6, 3, -1)$
- **Comparison:** $v \times u = -(u \times v)$

**Conclusion:** The cross product produces a vector perpendicular to both original vectors, and reversing the order of multiplication reverses the direction of the resulting vector while keeping its length unchanged.
