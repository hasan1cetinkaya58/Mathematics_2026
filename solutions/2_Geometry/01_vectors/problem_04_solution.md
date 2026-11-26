# Exercise 4. Dot Product and Perpendicularity

## Question

For $u=(1,2,-1)$ and $v=(2,-1,3)$, compute $u \cdot v$ and determine whether the vectors are perpendicular.

Then find $a$ so that $w=(2,-1,a)$ is perpendicular to $u$, and check the result.

> **Why this exercise:** Shows the dot product as both a test and a tool for constructing a perpendicularity condition.

## Solution

### 1. Computing the Dot Product

Given $u=(1,2,-1)$ and $v=(2,-1,3)$, the dot product is calculated by multiplying corresponding components and adding the results:

$$u \cdot v = u_1v_1 + u_2v_2 + u_3v_3$$

Substituting the given components:

$$u \cdot v = 1 \cdot 2 + 2 \cdot (-1) + (-1) \cdot 3 = 2 - 2 - 3 = -3$$

### 2. Determining Whether the Vectors Are Perpendicular

Two vectors are perpendicular if and only if their dot product equals zero ($u \cdot v = 0$). Since:

$$u \cdot v = -3 \neq 0$$

the vectors $u$ and $v$ are **not perpendicular**.

### 3. Finding the Value of $a$

We need to find $a$ such that $w=(2,-1,a)$ is perpendicular to $u=(1,2,-1)$, which requires $u \cdot w = 0$:

$$u \cdot w = 1 \cdot 2 + 2 \cdot (-1) + (-1) \cdot a = 2 - 2 - a = -a$$

Applying the perpendicularity condition:

$$-a = 0 \implies a = 0$$

### 4. Checking the Result

Substituting $a=0$ into $w$ gives $w=(2,-1,0)$. Recalculating the dot product:

$$u \cdot w = 1 \cdot 2 + 2 \cdot (-1) + (-1) \cdot 0 = 2 - 2 + 0 = 0$$

Since $u \cdot w = 0$, the vectors $u$ and $w$ are perpendicular.

## Final Results

- **First part:** $u \cdot v = -3 \neq 0$, so $u$ and $v$ are **not perpendicular**.
- **Second part:** $a = 0$, giving $w = (2,-1,0)$ with $u \cdot w = 0$, so $u$ and $w$ **are perpendicular**.

**Conclusion:** The dot product determines whether two vectors are perpendicular. In this exercise, the first pair of vectors is not perpendicular, while choosing $a=0$ makes the second pair perpendicular.
