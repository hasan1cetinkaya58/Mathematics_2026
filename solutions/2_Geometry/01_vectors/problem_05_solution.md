# Exercise 5. Angle Between Vectors

## Question

Given $u=(1,1,0)$ and $v=(1,0,1)$:

1. Use the sign of $u \cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

> **Why this exercise:** Teaches how to extract qualitative information first and only then perform the exact calculation.

## Solution

### 1. Predicting the Type of Angle

Given $u=(1,1,0)$ and $v=(1,0,1)$, we compute the dot product:

$$u \cdot v = 1 \cdot 1 + 1 \cdot 0 + 0 \cdot 1 = 1 + 0 + 0 = 1$$

Since $u \cdot v = 1 > 0$, the angle $\theta$ between the vectors is **acute** ($0^\circ \le \theta < 90^\circ$).

### 2. Computing the Angle

The formula for the angle $\theta$ between two vectors is:

$$\cos\theta = \frac{u \cdot v}{\|u\|\|v\|}$$

First, calculate the lengths of $u$ and $v$:

$$\|u\| = \sqrt{1^2 + 1^2 + 0^2} = \sqrt{1 + 1 + 0} = \sqrt{2}$$

$$\|v\| = \sqrt{1^2 + 0^2 + 1^2} = \sqrt{1 + 0 + 1} = \sqrt{2}$$

Substitute these values into the cosine formula:

$$\cos\theta = \frac{1}{\sqrt{2} \cdot \sqrt{2}} = \frac{1}{2}$$

Taking the inverse cosine:

$$\theta = \arccos\left(\frac{1}{2}\right) = 60^\circ \quad \left(\text{or } \frac{\pi}{3}\text{ rad}\right)$$

### 3. Comparing the Result with the Prediction

In Step 1, we predicted that the angle would be acute because $u \cdot v > 0$. The calculated angle is $\theta = 60^\circ$. Since $60^\circ < 90^\circ$, the angle is indeed acute, confirming our initial prediction.

## Final Results

- **Dot product:** $u \cdot v = 1 > 0$ (predicts an acute angle)
- **Magnitudes:** $\|u\| = \sqrt{2}$ and $\|v\| = \sqrt{2}$
- **Cosine of the angle:** $\cos\theta = \frac{1}{2}$
- **Angle:** $\theta = 60^\circ$ ($\frac{\pi}{3}\text{ rad}$)

**Conclusion:** The positive dot product indicates that the angle between the vectors is acute. The exact calculation gives $\theta = 60^\circ$, confirming the prediction.
