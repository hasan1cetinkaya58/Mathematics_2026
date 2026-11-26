# Exercise 3: Vector Normalization

## Question

For $v = (3, 4)$, find a unit vector $e$ with the same direction and orientation.

Check that $\|e\| = 1$, reconstruct $v$ in the form $v = \|v\|e$, and explain what changes during normalization and what remains unchanged.

## Solution

### 1. Finding the Length of the Vector

The given vector is $v = (3, 4)$. Its length is calculated using the formula:

$$\|v\| = \sqrt{x^2 + y^2}$$

Substituting the coordinates:

$$\|v\| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5$$

### 2. Finding the Unit Vector

To normalize a vector, we divide each component of the vector by its length:

$$e = \frac{v}{\|v\|}$$

Substituting the given vector and its length:

$$e = \frac{(3, 4)}{5} = \left(\frac{3}{5}, \frac{4}{5}\right)$$

### 3. Checking That the Unit Vector Has Length $1$

A unit vector must have a length equal to $1$:

$$\|e\| = \sqrt{\left(\frac{3}{5}\right)^2 + \left(\frac{4}{5}\right)^2} = \sqrt{\frac{9}{25} + \frac{16}{25}} = \sqrt{\frac{25}{25}} = \sqrt{1} = 1$$

This confirms that $e$ is a unit vector.

### 4. Reconstructing the Original Vector

We verify that the original vector can be reconstructed using $v = \|v\|e$:

$$v = 5\left(\frac{3}{5}, \frac{4}{5}\right) = \left(5 \cdot \frac{3}{5},\ 5 \cdot \frac{4}{5}\right) = (3, 4)$$

This is the exact original vector, so $v = \|v\|e$ holds.

### 5. Explaining What Changes and What Remains Unchanged

During normalization, the length of the vector changes from $\|v\| = 5$ to $\|e\| = 1$. However, the direction and orientation remain unchanged because both components are divided by the same positive scalar ($5 > 0$).

- **What changes:** The magnitude changes from $5$ to $1$.
- **What remains unchanged:** The direction and orientation of the vector.

## Final Results

- **Original vector:** $v = (3, 4)$
- **Length of the original vector:** $\|v\| = 5$
- **Normalized unit vector:** $e = \left(\frac{3}{5}, \frac{4}{5}\right)$
- **Length of the unit vector:** $\|e\| = 1$
- **Reconstructed original vector:** $v = 5\left(\frac{3}{5}, \frac{4}{5}\right) = (3, 4)$

**Conclusion:** The normalized vector has length $1$ while preserving the original vector's direction and orientation. Multiplying the unit vector by the original magnitude reconstructs the original vector exactly.
