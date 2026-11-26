
## Exercise 9: Cross Product as a Perpendicular Direction

### Question

Given the vectors:

`u = (1, 2, 0)` and `v = (0, 1, 3)`

1. Compute `u × v`.
2. Use dot products to check perpendicularity to both vectors.
3. Compute `v × u`.
4. Compare the results.

---

### Solution

### 1. Computing the Cross Product `u × v`

The cross product of two vectors in three-dimensional space produces a new vector that is perpendicular to both original vectors.

The cross product formula is:

`u × v = (u2*v3 - u3*v2, u3*v1 - u1*v3, u1*v2 - u2*v1)`

Given:

`u = (1, 2, 0)` and `v = (0, 1, 3)`

Substituting the components:

`u × v = (2*3 - 0*1, 0*0 - 1*3, 1*1 - 2*0)`

Calculating each component:

`u × v = (6, -3, 1)`

Therefore:

`u × v = (6, -3, 1)`

### 2. Checking Perpendicularity Using Dot Products

To verify that the cross product is perpendicular to both original vectors, we calculate two dot products.

A vector is perpendicular to another vector if their dot product is zero.

First, check perpendicularity to `u`.

We have:

`u = (1, 2, 0)`

`u × v = (6, -3, 1)`

Calculate the dot product:

`(u × v) · u = 6*1 + (-3)*2 + 1*0`

Simplifying:

`(u × v) · u = 6 - 6 + 0`

`(u × v) · u = 0`

Therefore, the cross product is perpendicular to `u`.

Now, check perpendicularity to `v`.

We have:

`v = (0, 1, 3)`

Calculate the dot product:

`(u × v) · v = 6*0 + (-3)*1 + 1*3`

Simplifying:

`(u × v) · v = 0 - 3 + 3`

`(u × v) · v = 0`

The cross product is also perpendicular to `v`.

Both checks confirm the perpendicularity of the result.

### 3. Computing the Cross Product `v × u`

Now we reverse the order of the original vectors.

Using the cross product formula:

`v × u = (v2*u3 - v3*u2, v3*u1 - v1*u3, v1*u2 - v2*u1)`

Substituting the components:

`v × u = (1*0 - 3*2, 3*1 - 0*0, 0*2 - 1*1)`

Calculating each component:

`v × u = (-6, 3, -1)`

Therefore:

`v × u = (-6, 3, -1)`

### 4. Comparing the Results

From our calculations:

`u × v = (6, -3, 1)`

`v × u = (-6, 3, -1)`

Comparing the two results, we can see that every component has the opposite sign.

Therefore:

`v × u = -(u × v)`

This demonstrates that the cross product is anti-commutative.

Changing the order of the vectors reverses the direction of the resulting vector, but its length remains unchanged.

Geometrically, both results are perpendicular to the same two original vectors, but they point in opposite directions.

---

### Final Results

**Cross product:**

`u × v = (6, -3, 1)`

**Perpendicularity checks:**

`(u × v) · u = 0`

`(u × v) · v = 0`

**Reversed cross product:**

`v × u = (-6, 3, -1)`

**Comparison:**

`v × u = -(u × v)`

**Conclusion:**

The cross product produces a vector perpendicular to both original vectors. Reversing the order of the vectors changes the direction of the result but preserves its magnitude. This shows that the cross product is anti-commutative.
