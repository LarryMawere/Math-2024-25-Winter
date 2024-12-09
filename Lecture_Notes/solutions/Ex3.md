## 11. Vectors I

1. By what number should vector \( {a = [3,4]} \) be multiplied so that its length is equal to \(1\)?}

The length of \( {a} = [3,4] \) is:
$$
\|\mathbf{a}\| = \sqrt{3^2 + 4^2} = 5
$$
To normalize:
$$
k \cdot \|\mathbf{a}\| = 1 \quad \implies \quad k = \frac{1}{5}
$$
Thus, the vector should be multiplied by \( \frac{1}{5}).

---

2. Calculate the length of vector \( {b = [1,1]} \) and find its unit vector.

{Length:}
$$
\|\mathbf{b}\| = \sqrt{1^2 + 1^2} = \sqrt{2}
$$

{Unit vector:}
$$
\mathbf{b_u} = \frac{\mathbf{b}}{\|\mathbf{b}\|} = \left[\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}\right]
$$

---

3. Plot the vector and the unit vector.


---

4. Calculate the length of vector \( \mathbf{c = [1,2,3]} \) and find its unit vector.

{Length:}
$$
\|\mathbf{c}\| = \sqrt{1^2 + 2^2 + 3^2} = \sqrt{14}
$$

{Unit vector:}
$$
\mathbf{c_u} = \frac{\mathbf{c}}{\|\mathbf{c}\|} = \left[\frac{1}{\sqrt{14}}, \frac{2}{\sqrt{14}}, \frac{3}{\sqrt{14}}\right]
$$

---

5. Find the Cartesian coordinates of \( {v = [2,3,4]} \) in the basis \( {b_1 = [1,0,1]}, {b_2 = [0,1,0]}, {b_3 = [1,0,-1]} \).

Let:
$$
\mathbf{v} = x_1 \mathbf{b_1} + x_2 \mathbf{b_2} + x_3 \mathbf{b_3}
$$
The equations are:
$$
x_1 + x_3 = 2, \quad x_2 = 3, \quad x_1 - x_3 = 4
$$
Adding and solving:
$$
x_1 = 3, \; x_2 = 3, \; x_3 = -1
$$
Thus, the coordinates are \( [3, 3, -1] \).

---

## 12. Vectors II

1. Perform the addition of \( [2,1] \) and \( [-1,1] \). Plot both vectors and their sum.

Addition:
$$
\mathbf{u} + \mathbf{v} = [2 + (-1), 1 + 1] = [1, 2]
$$

---

2. Calculate the area of the triangle spanned by vectors \( [2,1] \) and \( [-1,1] \).

Area:
$$
\text{Area} = \frac{1}{2} \left| \mathbf{u} \times \mathbf{v} \right|
$$
$$
\mathbf{u} \times \mathbf{v} = (2)(1) - (1)(-1) = 3
$$
$$
\text{Area} = \frac{1}{2} |3| = \frac{3}{2}
$$

---

3. Calculate the volume of the parallelepiped spanned by \( [2,1], [-1,1], [1,2] \).

Volume:
$$
\text{Volume} = \left| \mathbf{u} \cdot (\mathbf{v} \times \mathbf{w}) \right|
$$
Compute:
$$
\mathbf{v} \times \mathbf{w} = [0, 0, -3], \quad \mathbf{u} = [2, 1, 0]
$$
$$
\mathbf{u} \cdot (\mathbf{v} \times \mathbf{w}) = 0 \quad \implies \quad \text{Volume} = 0
$$

---

4. Check if vectors \( [2,1] \) and \( [-1,1] \) are perpendicular.

Dot product:
$$
\mathbf{u} \cdot \mathbf{v} = (2)(-1) + (1)(1) = -2 + 1 = -1
$$
Since \( {u} \cdot {v} \neq 0 \), they are not perpendicular.

---

5. Calculate the angle between \( [4,2,1] \) and \( [1,3,2] \).

Cosine of the angle:
$$
\cos \theta = \frac{\mathbf{u} \cdot \mathbf{v}}{\|\mathbf{u}\| \|\mathbf{v}\|}
$$
Compute:
$$
\mathbf{u} \cdot \mathbf{v} = 4(1) + 2(3) + 1(2) = 12, \quad \|\mathbf{u}\| = \sqrt{21}, \quad \|\mathbf{v}\| = \sqrt{14}
$$
$$
\cos \theta = \frac{12}{\sqrt{21} \sqrt{14}}
$$
Angle:
$$
\theta = \cos^{-1} \left( \frac{12}{\sqrt{21} \sqrt{14}} \right)
$$




---

## 13. Vectors III

1. Divide the line segment connecting \( A(-1,2) \) and \( B(3,-2) \) in the ratio \( 1:3 \).

Point:
$$
P = \frac{1 \cdot B + 3 \cdot A}{1 + 3} = \frac{1 \cdot (3,-2) + 3 \cdot (-1,2)}{4} = \frac{(3,-2) + (-3,6)}{4} = \frac{(0,4)}{4} = (0,1)
$$

---

## 14. Equations of Lines on a Plane

1. The line passes through points \( A(1,2) \) and \( B(3,4) \). Find the equation of the line.

Slope:
$$
m = \frac{y_2 - y_1}{x_2 - x_1} = \frac{4 - 2}{3 - 1} = 1
$$
Equation:
$$
y - 2 = 1(x - 1) \quad \implies \quad y = x + 1
$$

---

2. The line passes through point \( A(1,2) \) and is parallel to \( y = 2x + 3 \).

Same slope (\( m = 2 \)):
$$
y - 2 = 2(x - 1) \quad \implies \quad y = 2x
$$

---

3. The line passes through \( A(1,2) \) and is perpendicular to \( y = 2x + 3 \).

Perpendicular slope \( m = -\frac{1}{2} \):
$$
y - 2 = -\frac{1}{2}(x - 1) \quad \implies \quad y = -\frac{1}{2}x + \frac{5}{2}
$$

---
4. We have two lines \( y = 2x + 3 \) and \( y = 3x + 2 \). Find their intersection point and angle.

Intersection:
$$
x = 1, \; y = 5 \quad \text{(Point: \( (1,5) \))}
$$
Angle:
$$
\tan \theta = \frac{1}{7}, \quad \theta = \tan^{-1} \frac{1}{7}
$$

---
{5. Find a line parallel to \( {v = [2,3]} \) through \( A(1,2) \):}
$$
y = \frac{3}{2}x
$$

