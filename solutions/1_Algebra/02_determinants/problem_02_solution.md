# Determinants – Exercise 2

## Exercise 2. Determinant of a 3×3 Matrix

Given:

$$A=\begin{pmatrix}1&2&-1\\0&3&4\\2&1&5\end{pmatrix}$$

We will use Sarrus' rule.

### Step 1: Repeat the first two columns.

$$\begin{array}{ccc|cc}1&2&-1&1&2\\0&3&4&0&3\\2&1&5&2&1\end{array}$$

### Step 2: Add the downward diagonal products.

$$1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1=15+16+0=31$$

### Step 3: Add the upward diagonal products.

$$(-1)\cdot3\cdot2+2\cdot0\cdot5+1\cdot4\cdot1=-6+0+4=-2$$

### Step 4: Subtract the upward sum from the downward sum.

$$\det(A)=31-(-2)=\boxed{33}$$

### Step 5: Check using cofactor expansion along the first row.

$$\det(A)=1(15-4)-2(0-8)+(-1)(0-6)$$ $$=11+16+6=\boxed{33}$$



------------------------------------------------------------------------

