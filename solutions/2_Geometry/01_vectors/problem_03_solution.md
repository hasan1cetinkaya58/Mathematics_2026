## Exercise 3: Vector Normalization

### Question

Given the vector:

$$
v=(3,4)
$$

1. Find a unit vector \(e\) with the same direction and orientation.
2. Check that \(\|e\|=1\).
3. Reconstruct \(v\) in the form \(v=\|v\|e\).
4. Explain what changes during normalization and what remains unchanged.

---

### Solution

**1. Finding the Unit Vector**

A unit vector is a vector whose length (magnitude) is equal to 1.

To find a unit vector with the same direction and orientation as \(v\), we divide the original vector by its length.

The normalization formula is:

$$
e=\frac{v}{\|v\|}
$$

First, calculate the length of the given vector:

$$
v=(3,4)
$$

$$
\|v\|=\sqrt{3^2+4^2}
$$

$$
=\sqrt{9+16}
$$

$$
=\sqrt{25}=5
$$

Now divide each component of \(v\) by its length:

$$
e=\frac{(3,4)}{5}
$$

Therefore:

$$
\boxed{e=\left(\frac{3}{5},\frac{4}{5}\right)}
$$

**2. Checking That the Unit Vector Has Length 1**

To verify that \(e\) is a unit vector, we calculate its magnitude.

$$
\|e\|=\sqrt{\left(\frac{3}{5}\right)^2+
\left(\frac{4}{5}\right)^2}
$$

Squaring each component:

$$
=\sqrt{\frac{9}{25}+\frac{16}{25}}
$$

$$
=\sqrt{\frac{25}{25}}
$$

$$
=\sqrt{1}
$$

Therefore:

$$
\boxed{\|e\|=1}
$$

The result confirms that \(e\) is a unit vector.

**3. Reconstructing the Original Vector**

We need to express the original vector in the form:

$$
v=\|v\|e
$$

We already know that:

$$
\|v\|=5
$$

and

$$
e=\left(\frac{3}{5},\frac{4}{5}\right)
$$

Substituting these values:

$$
v=5\left(\frac{3}{5},\frac{4}{5}\right)
$$

Multiplying each component by 5:

$$
v=\left(5\cdot\frac{3}{5},
5\cdot\frac{4}{5}\right)
$$

$$
v=(3,4)
$$

Therefore:

$$
\boxed{v=5e=(3,4)}
$$

This confirms that the original vector can be reconstructed by multiplying its unit vector by its magnitude.

**4. Geometric Interpretation of Normalization**

Normalization separates the direction of a vector from its magnitude.

When a vector is normalized:

- Its magnitude changes to 1.
- Its direction remains unchanged.
- Its orientation remains unchanged.
- Its components are scaled proportionally.

In this exercise, the original vector has length 5. After normalization, its length becomes 1, but it still points in exactly the same direction.

Geometrically, normalization shortens the vector without rotating or reversing it.

---

### Final Results

$$
\boxed{\|v\|=5}
$$

$$
\boxed{e=\left(\frac{3}{5},\frac{4}{5}\right)}
$$

$$
\boxed{\|e\|=1}
$$

$$
\boxed{v=5e=(3,4)}
$$

**Conclusion:** Normalization changes the magnitude of a nonzero vector to 1 while preserving its direction and orientation. It allows us to represent a vector as the product of its length and a unit vector.
