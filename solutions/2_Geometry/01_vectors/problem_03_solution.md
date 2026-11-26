
# Exercise 3: Vector Normalization

## Question

For `v = (3, 4)`, find a unit vector `e` with the same direction and orientation.

Check that `|e| = 1`, reconstruct `v` in the form `v = |v|e`, and explain what changes during normalization and what remains unchanged.

## Solution

### 1. Finding the Length of the Vector

The given vector is:

`v = (3, 4)`

The length of a two-dimensional vector is calculated using the formula:

`|v| = sqrt(x^2 + y^2)`

Substituting the coordinates:

`|v| = sqrt(3^2 + 4^2)`

Calculating the squares:

`|v| = sqrt(9 + 16)`

Adding the values:

`|v| = sqrt(25)`

Therefore:

`|v| = 5`

### 2. Finding the Unit Vector

To normalize a vector, we divide each component of the vector by its length.

The normalization formula is:

`e = v / |v|`

Substituting the given vector and its length:

`e = (3, 4) / 5`

Dividing each component by 5:

`e = (3/5, 4/5)`

Therefore, the unit vector is:

`e = (3/5, 4/5)`

### 3. Checking That the Unit Vector Has Length 1

A unit vector must have a length equal to 1.

We use the length formula:

`|e| = sqrt(x^2 + y^2)`

Substituting the components of the unit vector:

`|e| = sqrt((3/5)^2 + (4/5)^2)`

Calculating the squares:

`|e| = sqrt(9/25 + 16/25)`

Adding the fractions:

`|e| = sqrt(25/25)`

Simplifying:

`|e| = sqrt(1)`

Therefore:

`|e| = 1`

This confirms that `e` is a unit vector.

### 4. Reconstructing the Original Vector

We need to verify that the original vector can be reconstructed using:

`v = |v|e`

We already know that:

`|v| = 5`

And:

`e = (3/5, 4/5)`

Substituting these values:

`v = 5(3/5, 4/5)`

Multiplying each component by 5:

`v = (5 * 3/5, 5 * 4/5)`

Simplifying:

`v = (3, 4)`

This is exactly the original vector.

Therefore:

`v = |v|e`

### 5. Explaining What Changes and What Remains Unchanged

During normalization, the length of the vector changes.

The original vector has length:

`|v| = 5`

The normalized vector has length:

`|e| = 1`

Therefore, normalization changes the magnitude of the vector to 1.

However, the direction and orientation remain unchanged because both components are divided by the same positive number.

The original vector and the unit vector point in the same direction.

Thus:
- **What changes:** The magnitude changes from 5 to 1.
- **What remains unchanged:** The direction and orientation of the vector.

## Final Results

Original vector:

`v = (3, 4)`

Length of the original vector:

`|v| = 5`

Normalized unit vector:

`e = (3/5, 4/5)`

Length of the unit vector:

`|e| = 1`

Reconstructed original vector:

`v = 5(3/5, 4/5) = (3, 4)`

**Conclusion:**

The normalized vector has length 1 while preserving the original vector's direction and orientation. Multiplying the unit vector by the original magnitude reconstructs the original vector exactly.

The exercise is solved correctly.
