
# Exercise 15: Comparing Directions Using the Cosine of the Angle

## Question

Given the vectors:

`a = (1, 2, 1)`, `b = (2, 4, 2)`, and `c = (2, 0, 3)`.

For each pair of vectors, compute the cosine of the angle using the formula:

`cos(theta) = (u · v) / (|u| |v|)`

1. Compute the cosine of the angle for each pair of vectors.
2. Order the pairs by increasing angle between the vectors.
3. Explain why for vectors `a` and `b`, the cosine value is `1` even though the vectors have different lengths.

## Solution

### 1. Calculating the Dot Products

We have three vectors, so we need to examine three pairs:

- Pair 1: `a` and `b`
- Pair 2: `a` and `c`
- Pair 3: `b` and `c`

First, calculate their dot products.

**For vectors `a` and `b`:**

`a · b = (1)(2) + (2)(4) + (1)(2)`

`a · b = 2 + 8 + 2 = 12`

**For vectors `a` and `c`:**

`a · c = (1)(2) + (2)(0) + (1)(3)`

`a · c = 2 + 0 + 3 = 5`

**For vectors `b` and `c`:**

`b · c = (2)(2) + (4)(0) + (2)(3)`

`b · c = 4 + 0 + 6 = 10`

### 2. Calculating the Vector Lengths

We use the Euclidean length formula:

`|v| = sqrt(x^2 + y^2 + z^2)`

**Length of vector `a`:**

`|a| = sqrt(1^2 + 2^2 + 1^2)`

`|a| = sqrt(1 + 4 + 1) = sqrt(6)`

**Length of vector `b`:**

`|b| = sqrt(2^2 + 4^2 + 2^2)`

`|b| = sqrt(4 + 16 + 4) = sqrt(24)`

`|b| = 2sqrt(6)`

**Length of vector `c`:**

`|c| = sqrt(2^2 + 0^2 + 3^2)`

`|c| = sqrt(4 + 0 + 9) = sqrt(13)`

### 3. Calculating the Cosine for Each Pair

We use the formula:

`cos(theta) = (u · v) / (|u| |v|)`

**Pair 1: Vectors `a` and `b`**

Substitute the calculated values:

`cos(theta_ab) = 12 / (sqrt(6) * 2sqrt(6))`

`cos(theta_ab) = 12 / 12`

`cos(theta_ab) = 1`

Since the cosine of zero degrees is 1:

`theta_ab = 0 degrees`

**Pair 2: Vectors `a` and `c`**

`cos(theta_ac) = 5 / (sqrt(6) * sqrt(13))`

`cos(theta_ac) = 5 / sqrt(78)`

`cos(theta_ac) ≈ 0.5661`

Therefore:

`theta_ac ≈ 55.4 degrees`

**Pair 3: Vectors `b` and `c`**

`cos(theta_bc) = 10 / (2sqrt(6) * sqrt(13))`

`cos(theta_bc) = 10 / (2sqrt(78))`

`cos(theta_bc) = 5 / sqrt(78)`

`cos(theta_bc) ≈ 0.5661`

Therefore:

`theta_bc ≈ 55.4 degrees`

### 4. Ordering the Pairs by Increasing Angle

The calculated angles are:

- Pair `(a, b)`: `0 degrees`
- Pair `(a, c)`: approximately `55.4 degrees`
- Pair `(b, c)`: approximately `55.4 degrees`

Therefore, the increasing order is:

`theta_ab < theta_ac = theta_bc`

The pairs `(a, c)` and `(b, c)` have equal angles because vectors `a` and `b` point in the same direction.

### 5. Geometric Explanation: Why Is the Cosine Equal to 1?

Notice that vector `b` is exactly twice vector `a`:

`b = 2a`

`(2, 4, 2) = 2(1, 2, 1)`

This means that the two vectors have the same direction, but different lengths.

Their angle is zero degrees:

`theta_ab = 0 degrees`

Since:

`cos(0 degrees) = 1`

The cosine value is 1 even though the vector lengths are different.

This demonstrates that the cosine formula measures the angle between vectors, not their lengths.

## Final Results

| Vector Pair | Cosine Value | Angle |
|---|---:|---:|
| `(a, b)` | `1` | `0 degrees` |
| `(a, c)` | `5/sqrt(78)` | `55.5 degrees` |
| `(b, c)` | `5/sqrt(78)` | `55.5 degrees` |

**Conclusion:**

The dot product and vector lengths together allow us to determine the angle between two vectors.

Vectors with different lengths can have the same direction. In this exercise, vectors `a` and `b` are parallel and point in the same direction, which is why their cosine value is exactly 1.
