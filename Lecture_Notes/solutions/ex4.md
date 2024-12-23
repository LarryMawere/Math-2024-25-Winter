# Solutions to Mathematical Problems

## 17. Equations of Second-Order Surfaces

### 1. Write the equation of a sphere with center at point \(P = (1, 2, 3)\) and radius \(r = 3\):
The general equation of a sphere is:
$$
(x - x_0)^2 + (y - y_0)^2 + (z - z_0)^2 = r^2
$$
Substituting \(P = (1, 2, 3)\) and \(r = 3\):
$$
(x - 1)^2 + (y - 2)^2 + (z - 3)^2 = 9
$$

---

### 2. Do the spheres \(x^2 + y^2 + z^2 = 1\) and \(x^2 + y^2 + z^2 = 2\) have any common points?
- Both spheres are centered at the origin \((0, 0, 0)\), with radii \(r_1 = 1\) and \(r_2 = \sqrt{2}\).
- Since the radii are different and both spheres are centered at the same point, they do not intersect.
- **Answer:** The spheres have no common points.

---

### 3. Intersection of spheres \(x^2 + y^2 + z^2 = 1\) and \((x - 1)^2 + y^2 + z^2 = 1\):
#### Step 1: Write equations
$$
x^2 + y^2 + z^2 = 1
$$
$$
(x - 1)^2 + y^2 + z^2 = 1
$$
#### Step 2: Expand the second equation
$$
(x - 1)^2 + y^2 + z^2 = x^2 - 2x + 1 + y^2 + z^2
$$
So:
$$
x^2 - 2x + 1 + y^2 + z^2 = 1
$$
#### Step 3: Subtract equations
$$
x^2 - 2x + 1 + y^2 + z^2 - (x^2 + y^2 + z^2) = 1 - 1
$$
Simplify:
$$
-2x + 1 = 0 \implies x = \frac{1}{2}
$$
#### Step 4: Substitute \(x = \frac{1}{2}\) into the first sphere equation
$$
\left(\frac{1}{2}\right)^2 + y^2 + z^2 = 1
$$
$$
\frac{1}{4} + y^2 + z^2 = 1
$$
$$
y^2 + z^2 = \frac{3}{4}
$$
This represents a **circle** in the plane \(x = \frac{1}{2}\) with radius:
$$
\sqrt{\frac{3}{4}} = \frac{\sqrt{3}}{2}
$$
**Answer:** The curve is a circle in the plane \(x = \frac{1}{2}\) with radius \(\frac{\sqrt{3}}{2}\).

---

### 4. Tangent plane to paraboloid \(z = (x - 1)^2 + y^2 + 1\) at \(P(1, 0, 1)\):
#### Formula for tangent plane
$$
z - z_0 = \frac{\partial f}{\partial x}(x - x_0) + \frac{\partial f}{\partial y}(y - y_0)
$$
#### Step 1: Compute partial derivatives
$$
\frac{\partial z}{\partial x} = 2(x - 1), \quad \frac{\partial z}{\partial y} = 2y
$$
At \(P(1, 0, 1)\):
$$
\frac{\partial z}{\partial x} = 0, \quad \frac{\partial z}{\partial y} = 0
$$
#### Step 2: Write equation
$$
z - 1 = 0(x - 1) + 0(y - 0)
$$
$$
z = 1
$$
**Answer:** The equation of the tangent plane is \(z = 1\).

---

## 18. Functions

### 1. Evaluate functions at \(x = 2\):
- \(f(x) = x^2 \implies f(2) = 2^2 = 4\)
- \(g(x) = \sqrt{x} \implies g(2) = \sqrt{2}\)
- \(h(x) = \frac{1}{x} \implies h(2) = \frac{1}{2}\)
- \(j(x) = \sin(x) \implies j(2) = \sin(2)\)

---

### 2. For \(f(x) = 3x - 1\) and \(g(x) = \sqrt{x}\):
1. \(f(g(x)) = f(\sqrt{x}) = 3\sqrt{x} - 1\)
2. \(g(f(x)) = g(3x - 1) = \sqrt{3x - 1}\)
3. \(f(f(x)) = f(3x - 1) = 3(3x - 1) - 1 = 9x - 4\)
4. \(g(g(x)) = g(\sqrt{x}) = \sqrt{\sqrt{x}} = x^{\frac{1}{4}}\)

---

### 3. For \(f(x) = e^x\) and \(g(x) = \ln(x)\):
- \(f(g(x)) = e^{\ln(x)} = x\)
- \(g(f(x)) = \ln(e^x) = x\)

**Observation:** \(f(x)\) and \(g(x)\) are inverses.

---

### 4. Inverse of \(f = \{(1, 7), (2, 9), (3, 11)\}\):
Swap inputs and outputs:
$$
f^{-1} = \{(7, 1), (9, 2), (11, 3)\}
$$

---

### 5. Inverse of \(f(x) = x - 1\):
Solve \(y = x - 1\) for \(x\):
$$
x = y + 1
$$
Thus:
$$
f^{-1}(x) = x + 1
$$


## **19. Limits of Sequences**

### **1. Calculate**

#### a. \(  \lim_{n \to \infty} \frac{n^2 + 3n}{2n^2 - 2n} \)

**Solution:**

1. Divide numerator and denominator by \(n^2\), the highest power of \(n\) in the denominator:
   $$
   \lim_{n \to \infty} \frac{n^2 + 3n}{2n^2 - 2n} = \lim_{n \to \infty} \frac{\frac{n^2}{n^2} + \frac{3n}{n^2}}{\frac{2n^2}{n^2} - \frac{2n}{n^2}}
   $$

2. Simplify:
   $$
   = \lim_{n \to \infty} \frac{1 + \frac{3}{n}}{2 - \frac{2}{n}}
   $$

3. As \(n \to \infty\), the terms \(\frac{3}{n}\) and \(\frac{2}{n}\) approach 0:
   $$
   = \frac{1 + 0}{2 - 0} = \frac{1}{2}
   $$

**Answer:** \(\frac{1}{2}\)

---

#### b. \( \lim_{n \to \infty} \frac{(2n + 3)^3}{n^3 - 1} \)

**Solution:**

1. Expand \((2n + 3)^3\) using the binomial theorem:
   $$
   (2n + 3)^3 = 8n^3 + 36n^2 + 54n + 27
   $$

2. Rewrite the limit:
   $$
   \lim_{n \to \infty} \frac{8n^3 + 36n^2 + 54n + 27}{n^3 - 1}
   $$

3. Divide numerator and denominator by \(n^3\):
   $$
   = \lim_{n \to \infty} \frac{\frac{8n^3}{n^3} + \frac{36n^2}{n^3} + \frac{54n}{n^3} + \frac{27}{n^3}}{\frac{n^3}{n^3} - \frac{1}{n^3}}
   $$

4. Simplify:
   $$
   = \lim_{n \to \infty} \frac{8 + \frac{36}{n} + \frac{54}{n^2} + \frac{27}{n^3}}{1 - \frac{1}{n^3}}
   $$

5. As \(n \to \infty\), the terms \(\frac{36}{n}\), \(\frac{54}{n^2}\), \(\frac{27}{n^3}\), and \(\frac{1}{n^3}\) approach 0:
   $$
   = \frac{8 + 0 + 0 + 0}{1 - 0} = 8
   $$

**Answer:** \(8\)

---

### **2. Prove using the squeeze theorem: \( \lim_{n \to \infty} \frac{\sin(n)}{n} = 0 \)**

**Solution:**

1. The sine function satisfies \(-1 \leq \sin(n) \leq 1\) for all \(n\).
2. Divide through by \(n > 0\):
   $$
   -\frac{1}{n} \leq \frac{\sin(n)}{n} \leq \frac{1}{n}
   $$

3. As \(n \to \infty\), both \(-\frac{1}{n}\) and \(\frac{1}{n}\) approach 0:
   $$
   \lim_{n \to \infty} -\frac{1}{n} = 0 \quad \text{and} \quad \lim_{n \to \infty} \frac{1}{n} = 0
   $$

4. By the squeeze theorem:
   $$
   \lim_{n \to \infty} \frac{\sin(n)}{n} = 0
   $$

**Answer:** \(0\)

---

### **3. Find the limit of the sequence: \( a_n = \left(1 + \frac{1}{n}\right)^n \)**

**Solution:**

The limit of this sequence is a well-known result:
$$
\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e
$$

**Answer:** \(e\)

---

## **20. Limits of Real Functions**

### **1. Compute \( \lim_{x \to \infty} \frac{x^2 + 2x}{x^4 - 3x^3} \)**

**Solution:**

1. Divide numerator and denominator by \(x^4\), the highest power of \(x\) in the denominator:
   $$
   \lim_{x \to \infty} \frac{x^2 + 2x}{x^4 - 3x^3} = \lim_{x \to \infty} \frac{\frac{x^2}{x^4} + \frac{2x}{x^4}}{\frac{x^4}{x^4} - \frac{3x^3}{x^4}}
   $$

2. Simplify:
   $$
   = \lim_{x \to \infty} \frac{\frac{1}{x^2} + \frac{2}{x^3}}{1 - \frac{3}{x}}
   $$

3. As \(x \to \infty\), the terms \(\frac{1}{x^2}\), \(\frac{2}{x^3}\), and \(\frac{3}{x}\) approach 0:
   $$
   = \frac{0 + 0}{1 - 0} = 0
   $$

**Answer:** \(0\)

---

### **2. Find \( \lim_{x \to 0} \frac{\sin(3x)}{2x + 1} \)**

**Solution:**

1. Direct substitution gives:
   $$
   \frac{\sin(3 \cdot 0)}{2 \cdot 0 + 1} = \frac{0}{1} = 0
   $$

**Answer:** \(0\)

---

### **3. Find the asymptotes of the functions**

#### a. \( f(x) = \frac{x^2 - 1}{x - 1} \)

**Solution:**

1. Factorize numerator:
   $$
   f(x) = \frac{(x - 1)(x + 1)}{x - 1}
   $$

2. Simplify (for \(x \neq 1\)):
   $$
   f(x) = x + 1
   $$

3. Vertical asymptote: At \(x = 1\) (denominator becomes 0).
4. No horizontal asymptote since \(f(x)\) simplifies to a linear function.

**Answer:**
- Vertical asymptote: \(x = 1\)

---

#### b. \( g(x) = \frac{1}{\sin(x)} \)

**Solution:**

1. Vertical asymptotes occur when \(\sin(x) = 0\):
   $$
   x = n\pi, \; n \in \mathbb{Z}
   $$

2. No horizontal asymptote since \(\frac{1}{\sin(x)}\) oscillates infinitely.

**Answer:**
- Vertical asymptotes: \(x = n\pi, \; n \in \mathbb{Z}\)
