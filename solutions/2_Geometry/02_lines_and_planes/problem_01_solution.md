
# Exercise 1. Line Through Two Points

## Question

**Given:**

Two points in the plane:

`A = (1, 2)` and `B = (4, -1)`.

**Required:**

1. Find the equation of the line in parametric form.
2. Find the equation of the line in general form.
3. Identify a direction vector and an example of a normal vector.
4. Check that both points satisfy the equation of the line.

## Solution

### 1. Finding the Direction Vector

A direction vector describes the direction in which a line moves.

Since the line passes through points `A` and `B`, we can find its direction vector by subtracting the coordinates of `A` from the coordinates of `B`.

The formula is:

`v = B - A`

Substitute the coordinates:

`v = (4 - 1, -1 - 2)`

Therefore:

`v = (3, -3)`

We can simplify this vector by dividing both components by `3`:

`v = (1, -1)`

Both vectors represent the same direction. We will use the simpler vector `v = (1, -1)` in the next steps.

### 2. Finding the Parametric Equation

The parametric form describes a line using:

- A known point on the line.
- A direction vector.
- A real parameter `t`.

The general formula is:

`(x, y) = A + t v`

We know that:

`A = (1, 2)`

`v = (1, -1)`

Substitute these values into the formula:

`(x, y) = (1, 2) + t(1, -1)`

Now compare the coordinates:

`x = 1 + t`

`y = 2 - t`

Therefore, the parametric equation of the line is:

`x = 1 + t`

`y = 2 - t`

where `t` can be any real number.

**Explanation:**

When `t = 0`, we get point `A = (1, 2)`.

When `t = 3`, we get point `B = (4, -1)`.

This shows that both given points lie on the parametric line.

### 3. Finding the General Equation

The general form of a line in two dimensions is:

`ax + by + c = 0`

To find this equation, we first calculate the slope of the line.

The slope formula is:

`m = (y2 - y1) / (x2 - x1)`

Using points `A = (1, 2)` and `B = (4, -1)`:

`m = (-1 - 2) / (4 - 1)`

`m = -3 / 3`

Therefore:

`m = -1`

Now we use the point-slope formula:

`y - y1 = m(x - x1)`

Substitute the slope and the coordinates of point `A`:

`y - 2 = -1(x - 1)`

Expand the right-hand side:

`y - 2 = -x + 1`

Move all terms to the left-hand side:

`x + y - 3 = 0`

Therefore, the general equation of the line is:

`x + y - 3 = 0`

### 4. Identifying a Normal Vector

A normal vector is perpendicular to the line.

For a line written in general form:

`ax + by + c = 0`

A normal vector can be obtained directly from the coefficients of `x` and `y`:

`n = (a, b)`

Our general equation is:

`x + y - 3 = 0`

The coefficients are:

`a = 1` and `b = 1`

Therefore, one example of a normal vector is:

`n = (1, 1)`

We can verify that the normal vector is perpendicular to the direction vector by calculating their dot product.

The direction vector is:

`v = (1, -1)`

The normal vector is:

`n = (1, 1)`

Their dot product is:

`v · n = (1)(1) + (-1)(1)`

`v · n = 1 - 1`

`v · n = 0`

Since the dot product is zero, the two vectors are perpendicular.

This confirms that `n = (1, 1)` is a valid normal vector.

### 5. Checking the Given Points

Finally, we substitute both given points into the general equation:

`x + y - 3 = 0`

If the equation is satisfied, the point lies on the line.

**Checking point A = (1, 2):**

Substitute `x = 1` and `y = 2`:

`1 + 2 - 3 = 0`

`0 = 0`

Therefore, point `A` satisfies the equation.

**Checking point B = (4, -1):**

Substitute `x = 4` and `y = -1`:

`4 + (-1) - 3 = 0`

`4 - 1 - 3 = 0`

`0 = 0`

Therefore, point `B` also satisfies the equation.

Both points satisfy the general equation, so the line passes through the two given points.

## Final Answer

- **Parametric form:**

  `x = 1 + t`

  `y = 2 - t`

- **General form:**

  `x + y - 3 = 0`

- **Direction vector:**

  `v = (1, -1)`

- **Normal vector:**

  `n = (1, 1)`

- **Verification:** Both points `A = (1, 2)` and `B = (4, -1)` satisfy the general equation.

Therefore, the required line has been correctly described in both parametric and general forms.
