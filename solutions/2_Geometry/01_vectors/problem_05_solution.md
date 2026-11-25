## Exercise 5: Angle Between Vectors

### Question

Given the vectors:

$$
u=(1,1,0), \qquad v=(1,0,1)
$$

1. Use the sign of \(u\cdot v\) to predict the type of angle.
2. Compute the angle between the vectors.
3. Compare the result with the prediction.

---

### Solution

**1. Predicting the Type of Angle Using the Dot Product**

First, calculate the dot product of the two vectors.

The dot product formula is:

$$
u\cdot v=u_1v_1+u_2v_2+u_3v_3
$$

Substituting the given vectors:

$$
u\cdot v=(1)(1)+(1)(0)+(0)(1)
$$

$$
=1+0+0
$$

$$
\boxed{u\cdot v=1}
$$

The sign of the dot product tells us the type of angle between two nonzero vectors:

- If the dot product is positive, the angle is acute.
- If the dot product is zero, the angle is right.
- If the dot product is negative, the angle is obtuse.

Since:

$$
u\cdot v=1>0
$$

We predict that the angle between the vectors is acute.

**2. Computing the Angle Between the Vectors**

To calculate the exact angle, we use the dot product formula:

$$
u\cdot v=\|u\|\|v\|\cos\theta
$$

Rearranging the formula to find the angle:

$$
\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}
$$

Therefore:

$$
\theta=\cos^{-1}\left(
\frac{u\cdot v}{\|u\|\|v\|}
\right)
$$

First, calculate the length of vector \(u\):

$$
\|u\|=\sqrt{1^2+1^2+0^2}
$$

$$
=\sqrt{1+1+0}
$$

$$
\|u\|=\sqrt{2}
$$

Next, calculate the length of vector \(v\):

$$
\|v\|=\sqrt{1^2+0^2+1^2}
$$

$$
=\sqrt{1+0+1}
$$

$$
\|v\|=\sqrt{2}
$$

Now substitute the values into the angle formula:

$$
\theta=\cos^{-1}\left(
\frac{1}{\sqrt{2}\cdot\sqrt{2}}
\right)
$$

Simplifying:

$$
=\cos^{-1}\left(\frac{1}{2}\right)
$$

Since:

$$
\cos 60^\circ=\frac{1}{2}
$$

We obtain:

$$
\boxed{\theta=60^\circ}
$$

**3. Comparing the Result with the Prediction**

In the first part, the dot product was positive:

$$
u\cdot v=1>0
$$

Therefore, we predicted that the angle would be acute.

In the second part, we calculated the exact angle:

$$
\theta=60^\circ
$$

Since:

$$
0^\circ<60^\circ<90^\circ
$$

The calculated angle is acute.

Therefore, the prediction is correct.

---

### Final Results

Dot product:

$$
\boxed{u\cdot v=1}
$$

Vector lengths:

$$
\boxed{\|u\|=\sqrt{2},\quad \|v\|=\sqrt{2}}
$$

Angle:

$$
\boxed{\theta=60^\circ}
$$

Prediction:

$$
\boxed{\text{Acute angle}}
$$

**Conclusion:** The sign of the dot product allows us to predict whether the angle between two nonzero vectors is acute, right, or obtuse. The dot product formula then gives us the exact angle. In this exercise, the positive dot product correctly predicted an acute angle of \(60^\circ\).
