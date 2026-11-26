
## Exercise 8: Linear Combination and Checking the Result

### Question

Given the vectors:

- `w = (5, 1)`
- `u = (1, 1)`
- `v = (2, -1)`

Check whether `w` can be written as:

`w = au + bv`

If so:

1. Find the values of `a` and `b`.
2. Reconstruct `w` using these coefficients.
3. Explain the geometric meaning of the existence of such coefficients.

---

### Solution

### 1. Finding the Coefficients `a` and `b`

We want to determine whether `w` can be expressed as a linear combination of `u` and `v`.

The given equation is:

`w = au + bv`

Substituting the given vectors:

`(5, 1) = a(1, 1) + b(2, -1)`

First, multiply each vector by its corresponding scalar:

`(5, 1) = (a, a) + (2b, -b)`

Adding the corresponding components gives:

`(5, 1) = (a + 2b, a - b)`

By comparing the corresponding components, we obtain the following system of equations:

`a + 2b = 5`

`a - b = 1`

Now solve the system.

Subtract the second equation from the first equation:

`(a + 2b) - (a - b) = 5 - 1`

Simplifying:

`a + 2b - a + b = 4`

`3b = 4`

Therefore:

`b = 4/3`

Now substitute this value into the second equation:

`a - 4/3 = 1`

Adding `4/3` to both sides:

`a = 1 + 4/3`

Therefore:

`a = 7/3`

The required coefficients are:

`a = 7/3` and `b = 4/3`

### 2. Reconstructing the Original Vector

To verify our solution, substitute the calculated coefficients into the original linear combination.

We have:

`w = au + bv`

Substituting the values:

`w = (7/3)(1, 1) + (4/3)(2, -1)`

Multiply each vector by its coefficient:

`w = (7/3, 7/3) + (8/3, -4/3)`

Add the corresponding components:

`w = (7/3 + 8/3, 7/3 - 4/3)`

Simplifying:

`w = (15/3, 3/3)`

Therefore:

`w = (5, 1)`

This is exactly the original vector, so our calculations are correct.

### 3. Geometric Interpretation

A linear combination means creating a new vector by scaling and adding other vectors.

In this exercise:

- Vector `u` is scaled by `7/3`.
- Vector `v` is scaled by `4/3`.
- The two resulting vectors are added together to produce `w`.

Geometrically, the coefficients determine how far and in which direction each vector contributes to the resulting vector.

Since `u = (1, 1)` and `v = (2, -1)` are not scalar multiples of each other, they point in different directions.

Therefore, they span the entire two-dimensional plane `R^2`.

This means that every vector in `R^2`, including `w = (5, 1)`, can be represented as a linear combination of `u` and `v`.

In this case, the coefficients are also unique because the two given vectors are linearly independent.

---

### Final Results

**Coefficients:**

`a = 7/3` and `b = 4/3`

**Linear combination:**

`w = (7/3)u + (4/3)v`

**Verification:**

`(5, 1) = (5, 1)`

**Final conclusion:**

Yes, `w` can be expressed as a linear combination of `u` and `v`.

Since `u` and `v` are linearly independent and span `R^2`, the vector `w` can be represented uniquely using the coefficients `a = 7/3` and `b = 4/3`.
