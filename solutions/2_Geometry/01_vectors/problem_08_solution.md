## Exercise 8: Linear Combination and Checking the Result

### Question

Given the vectors:

$$
w=(5,1)
$$

$$
u=(1,1), \qquad v=(2,-1)
$$

Check whether \(w\) can be written as:

$$
w=au+bv
$$

If so:

1. Find the values of \(a\) and \(b\).
2. Reconstruct \(w\) using these coefficients.
3. Explain the geometric meaning of the existence of such coefficients.

---

### Solution

**1. Finding the Coefficients \(a\) and \(b\)**

We want to determine whether \(w\) can be expressed as a linear combination of \(u\) and \(v\).

The given equation is:

$$
w=au+bv
$$

Substituting the given vectors:

$$
(5,1)=a(1,1)+b(2,-1)
$$

First, multiply each vector by its corresponding scalar:

$$
(5,1)=(a,a)+(2b,-b)
$$

Adding the corresponding components gives:

$$
(5,1)=(a+2b,a-b)
$$

By comparing the corresponding components, we obtain the following system of equations:

$$
a+2b=5
$$

$$
a-b=1
$$

Now solve the system.

Subtract the second equation from the first equation:

$$
(a+2b)-(a-b)=5-1
$$

Simplifying:

$$
a+2b-a+b=4
$$

$$
3b=4
$$

Therefore:

$$
\boxed{b=\frac{4}{3}}
$$

Now substitute this value into the second equation:

$$
a-\frac{4}{3}=1
$$

Adding \(\frac{4}{3}\) to both sides:

$$
a=1+\frac{4}{3}
$$

$$
\boxed{a=\frac{7}{3}}
$$

Therefore, the required coefficients are:

$$
\boxed{a=\frac{7}{3}, \qquad b=\frac{4}{3}}
$$

**2. Reconstructing the Original Vector**

To verify our solution, substitute the calculated coefficients into the original linear combination.

We have:

$$
w=au+bv
$$

Substituting the values:

$$
w=\frac{7}{3}(1,1)+\frac{4}{3}(2,-1)
$$

Multiply each vector by its coefficient:

$$
w=\left(\frac{7}{3},\frac{7}{3}\right)
+\left(\frac{8}{3},-\frac{4}{3}\right)
$$

Add the corresponding components:

$$
w=\left(
\frac{7}{3}+\frac{8}{3},
\frac{7}{3}-\frac{4}{3}
\right)
$$

Simplifying:

$$
w=\left(\frac{15}{3},\frac{3}{3}\right)
$$

Therefore:

$$
\boxed{w=(5,1)}
$$

This is exactly the original vector, so our calculations are correct.

**3. Geometric Interpretation**

A linear combination means creating a new vector by scaling and adding other vectors.

In this exercise:

- Vector \(u\) is scaled by \(\frac{7}{3}\).
- Vector \(v\) is scaled by \(\frac{4}{3}\).
- The two resulting vectors are added together to produce \(w\).

Geometrically, the coefficients determine how far and in which direction each vector contributes to the resulting vector.

Since \(u=(1,1)\) and \(v=(2,-1)\) are not scalar multiples of each other, they point in different directions.

Therefore, they span the entire two-dimensional plane \(\mathbb{R}^2\).

This means that every vector in \(\mathbb{R}^2\), including \(w=(5,1)\), can be represented as a linear combination of \(u\) and \(v\).

In this case, the coefficients are also unique because the two given vectors are linearly independent.

---

### Final Results

Coefficients:

$$
\boxed{a=\frac{7}{3}, \qquad b=\frac{4}{3}}
$$

Linear combination:

$$
\boxed{w=\frac{7}{3}u+\frac{4}{3}v}
$$

Verification:

$$
\boxed{(5,1)=(5,1)}
$$

Final conclusion:

$$
\boxed{\text{Yes, }w\text{ can be expressed as a linear combination of }u\text{ and }v.}
$$

**Conclusion:** A linear combination allows us to construct new vectors by scaling and adding existing vectors. Since \(u\) and \(v\) are linearly independent and span \(\mathbb{R}^2\), the vector \(w\) can be represented uniquely using the coefficients \(a=\frac{7}{3}\) and \(b=\frac{4}{3}\).
