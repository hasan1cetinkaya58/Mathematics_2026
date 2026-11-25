# Exercise 15: Comparing Directions Using the Cosine of the Angle

## Question

Given the vectors:

$$
a=(1,2,1), \quad b=(2,4,2), \quad c=(2,0,3)
$$

For each pair of vectors, compute the cosine of the angle using the formula:

$$
\cos\theta=\frac{u\cdot v}{|u||v|}
$$

Order the pairs by increasing angle between the vectors.

Explain why for vectors \(a\) and \(b\), the cosine value is \(1\) even though the vectors have different lengths.

## Solution

### 1. Calculating the Dot Products

We have three vectors, so we need to examine three pairs:

- Pair 1: \(a\) and \(b\)
- Pair 2: \(a\) and \(c\)
- Pair 3: \(b\) and \(c\)

First, calculate their dot products.

**For vectors \(a\) and \(b\):**

$$
a\cdot b=(1)(2)+(2)(4)+(1)(2)
$$

$$
a\cdot b=2+8+2=12
$$

**For vectors \(a\) and \(c\):**

$$
a\cdot c=(1)(2)+(2)(0)+(1)(3)
$$

$$
a\cdot c=2+0+3=5
$$

**For vectors \(b\) and \(c\):**

$$
b\cdot c=(2)(2)+(4)(0)+(2)(3)
$$

$$
b\cdot c=4+0+6=10
$$

### 2. Calculating the Vector Lengths

We use the Euclidean length formula:

$$
|v|=\sqrt{x^2+y^2+z^2}
$$

**Length of vector \(a\):**

$$
|a|=\sqrt{1^2+2^2+1^2}
$$

$$
|a|=\sqrt{1+4+1}=\sqrt{6}
$$

**Length of vector \(b\):**

$$
|b|=\sqrt{2^2+4^2+2^2}
$$

$$
|b|=\sqrt{4+16+4}=\sqrt{24}
$$

$$
|b|=2\sqrt{6}
$$

**Length of vector \(c\):**

$$
|c|=\sqrt{2^2+0^2+3^2}
$$

$$
|c|=\sqrt{4+0+9}=\sqrt{13}
$$

### 3. Calculating the Cosine for Each Pair

We use the formula:

$$
\cos\theta=\frac{u\cdot v}{|u||v|}
$$

**Pair 1: Vectors \(a\) and \(b\)**

Substitute the calculated values:

$$
\cos\theta_{ab}=
\frac{12}{\sqrt{6}\cdot 2\sqrt{6}}
$$

$$
\cos\theta_{ab}=\frac{12}{12}
$$

$$
\boxed{\cos\theta_{ab}=1}
$$

Since the cosine of zero degrees is 1:

$$
\boxed{\theta_{ab}=0^\circ}
$$

**Pair 2: Vectors \(a\) and \(c\)**

$$
\cos\theta_{ac}=
\frac{5}{\sqrt{6}\cdot\sqrt{13}}
$$

$$
\cos\theta_{ac}=\frac{5}{\sqrt{78}}
$$

$$
\boxed{\cos\theta_{ac}\approx 0.5661}
$$

Therefore:

$$
\boxed{\theta_{ac}\approx 55.4^\circ}
$$

**Pair 3: Vectors \(b\) and \(c\)**

$$
\cos\theta_{bc}=
\frac{10}{2\sqrt{6}\cdot\sqrt{13}}
$$

$$
\cos\theta_{bc}=\frac{10}{2\sqrt{78}}
$$

$$
\boxed{\cos\theta_{bc}=\frac{5}{\sqrt{78}}}
$$

$$
\boxed{\cos\theta_{bc}\approx 0.5661}
$$

Therefore:

$$
\boxed{\theta_{bc}\approx 55.4^\circ}
$$

### 4. Ordering the Pairs by Increasing Angle

The calculated angles are:

- Pair \((a,b)\): \(0^\circ\)
- Pair \((a,c)\): approximately \(55.4^\circ\)
- Pair \((b,c)\): approximately \(55.4^\circ\)

Therefore, the increasing order is:

$$
\boxed{(a,b)<(a,c)=(b,c)}
$$

The pairs \((a,c)\) and \((b,c)\) have equal angles because vectors \(a\) and \(b\) point in the same direction.

### 5. Geometric Explanation: Why Is the Cosine Equal to 1?

Notice that vector \(b\) is exactly twice vector \(a\):

$$
b=2a
$$

$$
(2,4,2)=2(1,2,1)
$$

This means that the two vectors have the same direction, but different lengths.

Their angle is zero degrees:

$$
\theta_{ab}=0^\circ
$$

Since:

$$
\cos(0^\circ)=1
$$

The cosine value is 1 even though the vector lengths are different.

This demonstrates that the cosine formula measures the angle between vectors, not their lengths.

## Final Results

| Vector Pair | Cosine Value | Angle |
|---|---:|---:|
| \((a,b)\) | \(1\) | \(0^\circ\) |
| \((a,c)\) | \(5/\sqrt{78}\) | \(55.4^\circ\) |
| \((b,c)\) | \(5/\sqrt{78}\) | \(55.4^\circ\) |

**Conclusion:**

The dot product and vector lengths together allow us to determine the angle between two vectors.

Vectors with different lengths can have the same direction. In this exercise, vectors \(a\) and \(b\) are parallel and point in the same direction, which is why their cosine value is exactly 1.
