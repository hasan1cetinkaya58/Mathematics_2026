# Exercise 15: Comparing Directions Using the Cosine of the Angle

## Question

Given the vectors:

$$a = (1, 2, 1), \qquad b = (2, 4, 2), \qquad c = (2, 0, 3)$$

For each pair of vectors, compute the cosine of the angle using the formula:

$$\cos\theta = \frac{u \cdot v}{\|u\|\|v\|}$$

1. Compute the cosine of the angle for each pair of vectors.
2. Order the pairs by increasing angle between the vectors.
3. Explain why for vectors $a$ and $b$, the cosine value is $1$ even though the vectors have different lengths.

## Solution

### 1. Calculating the Dot Products

We have three vectors, so we examine three pairs: $(a, b)$, $(a, c)$, and $(b, c)$.

- **For vectors $a$ and $b$:**

$$a \cdot b = (1)(2) + (2)(4) + (1)(2) = 2 + 8 + 2 = 12$$

- **For vectors $a$ and $c$:**

$$a \cdot c = (1)(2) + (2)(0) + (1)(3) = 2 + 0 + 3 = 5$$

- **For vectors $b$ and $c$:**

$$b \cdot c = (2)(2) + (4)(0) + (2)(3) = 4 + 0 + 6 = 10$$

### 2. Calculating the Vector Lengths

Using the Euclidean length formula $\|v\| = \sqrt{x^2 + y^2 + z^2}$:

- **Length of vector $a$:**

$$\|a\| = \sqrt{1^2 + 2^2 + 1^2} = \sqrt{1 + 4 + 1} = \sqrt{6}$$

- **Length of vector $b$:**

$$\|b\| = \sqrt{2^2 + 4^2 + 2^2} = \sqrt{4 + 16 + 4} = \sqrt{24} = 2\sqrt{6}$$

- **Length of vector $c$:**

$$\|c\| = \sqrt{2^2 + 0^2 + 3^2} = \sqrt{4 + 0 + 9} = \sqrt{13}$$

### 3. Calculating the Cosine for Each Pair

Using $\cos\theta = \dfrac{u \cdot v}{\|u\|\|v\|}$:

- **Pair 1: Vectors $a$ and $b$**

$$\cos\theta_{ab} = \frac{12}{\sqrt{6} \cdot 2\sqrt{6}} = \frac{12}{12} = 1$$

Since $\cos 0^\circ = 1$, we obtain:

$$\theta_{ab} = 0^\circ$$

- **Pair 2: Vectors $a$ and $c$**

$$\cos\theta_{ac} = \frac{5}{\sqrt{6} \cdot \sqrt{13}} = \frac{5}{\sqrt{78}} \approx 0.5661$$

Taking the inverse cosine:

$$\theta_{ac} = \arccos\left(\frac{5}{\sqrt{78}}\right) \approx 55.5^\circ$$

- **Pair 3: Vectors $b$ and $c$**

$$\cos\theta_{bc} = \frac{10}{2\sqrt{6} \cdot \sqrt{13}} = \frac{10}{2\sqrt{78}} = \frac{5}{\sqrt{78}} \approx 0.5661$$

Taking the inverse cosine:

$$\theta_{bc} = \arccos\left(\frac{5}{\sqrt{78}}\right) \approx 55.5^\circ$$

### 4. Ordering the Pairs by Increasing Angle

The calculated angles are:

- Pair $(a, b)$: $\theta_{ab} = 0^\circ$
- Pair $(a, c)$: $\theta_{ac} \approx 55.5^\circ$
- Pair $(b, c)$: $\theta_{bc} \approx 55.5^\circ$

Therefore, the increasing order is:

$$\theta_{ab} < \theta_{ac} = \theta_{bc}$$

The pairs $(a, c)$ and $(b, c)$ have equal angles because $a$ and $b$ point in the same direction.

### 5. Geometric Explanation: Why Is the Cosine Equal to $1$?

Notice that $b$ is a positive scalar multiple of $a$:

$$b = 2a \iff (2, 4, 2) = 2(1, 2, 1)$$

This means $a$ and $b$ point in the exact same direction while having different magnitudes ($\|b\| = 2\|a\|$). Consequently, the angle between them is $\theta_{ab} = 0^\circ$, and since $\cos 0^\circ = 1$, their cosine value equals $1$. Because the cosine formula normalizes each vector by its length ($\frac{u}{\|u\|}$ and $\frac{v}{\|v\|}$), it depends solely on direction, not magnitude.

## Final Results

| Vector Pair | Cosine Value | Angle |
|---|---:|---:|
| $(a, b)$ | $1$ | $0^\circ$ |
| $(a, c)$ | $\dfrac{5}{\sqrt{78}} \approx 0.5661$ | $\approx 55.5^\circ$ |
| $(b, c)$ | $\dfrac{5}{\sqrt{78}} \approx 0.5661$ | $\approx 55.5^\circ$ |

**Conclusion:** The dot product and vector lengths together determine the angle between two vectors. Vectors with different lengths can share the same direction; here, $a$ and $b$ are parallel with the same orientation, so $\cos\theta_{ab} = 1$.
