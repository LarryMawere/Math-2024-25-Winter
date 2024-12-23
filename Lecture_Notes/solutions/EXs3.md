# Equations of Planes in Space

### 1. The plane passes through points \( A(1, 2, 3) \), \( B(3, 4, 5) \), and \( C(2, 1, 4) \). Find the equation of the plane.

To find the equation of the plane passing through three points, we first need to calculate two vectors that lie in the plane. These vectors can be obtained from the given points:

- Vector \( \overrightarrow{AB} = B - A = (3 - 1, 4 - 2, 5 - 3) = (2, 2, 2) \)
- Vector \( \overrightarrow{AC} = C - A = (2 - 1, 1 - 2, 4 - 3) = (1, -1, 1) \)

Next, calculate the cross product of \( \overrightarrow{AB} \) and \( \overrightarrow{AC} \) to get the normal vector to the plane.

$$
\mathbf{n} = \overrightarrow{AB} \times \overrightarrow{AC} = 
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 2 & 2 \\
1 & -1 & 1
\end{vmatrix}
= \hat{i}(2 \cdot 1 - 2 \cdot (-1)) - \hat{j}(2 \cdot 1 - 2 \cdot 1) + \hat{k}(2 \cdot (-1) - 2 \cdot 1)
$$

Simplifying the determinant:

$$
\mathbf{n} = \hat{i}(4) - \hat{j}(0) + \hat{k}(-4)
$$

$$
\mathbf{n} = (4, 0, -4)
$$

Now, the equation of the plane is given by:

$$
4(x - 1) + 0(y - 2) - 4(z - 3) = 0
$$

Simplifying:

$$
4x - 4z = 4
$$

$$
x - z = 1
$$

Thus, the equation of the plane is \( x - z = 1 \).

---

### 2. The plane passes through point \( A(1, 2, 3) \) and is parallel to the plane \( 2x + 3y + 4z = 5 \). Find the equation of the plane.

If the plane is parallel to \( 2x + 3y + 4z = 5 \), then the normal vector of the required plane will be the same as the normal vector of this given plane. The normal vector of the plane \( 2x + 3y + 4z = 5 \) is \( \mathbf{n} = (2, 3, 4) \).

The equation of the plane passing through \( A(1, 2, 3) \) and parallel to this normal vector is:

$$
2(x - 1) + 3(y - 2) + 4(z - 3) = 0
$$

Expanding this:

$$
2x - 2 + 3y - 6 + 4z - 12 = 0
$$

$$
2x + 3y + 4z = 20
$$

Thus, the equation of the plane is \( 2x + 3y + 4z = 20 \).

---

### 3. The plane passes through point \( A(1, 2, 3) \) and is perpendicular to the normal vector \( n = [2, 3, 4] \). Find the equation of the plane.

The normal vector of the plane is \( \mathbf{n} = (2, 3, 4) \), and the plane passes through \( A(1, 2, 3) \). The equation of the plane is:

$$
2(x - 1) + 3(y - 2) + 4(z - 3) = 0
$$

Expanding this:

$$
2x - 2 + 3y - 6 + 4z - 12 = 0
$$

$$
2x + 3y + 4z = 20
$$

So, the equation of the plane is \( 2x + 3y + 4z = 20 \), which is the same as the previous one.

---

### 4. We have two planes \( 2x + 3y + 4z = 5 \) and \( 3x + 4y + 2z = 6 \). Find the line of intersection of these planes.

The equations of the planes are:

$$
2x + 3y + 4z = 5 \quad \text{(Plane 1)}
$$

$$
3x + 4y + 2z = 6 \quad \text{(Plane 2)}
$$

To solve, let's use elimination or substitution. We can eliminate one of the variables. For simplicity, we'll eliminate \( z \).

Multiply the first equation by 3 and the second equation by 2:

$$
6x + 9y + 12z = 15 \quad \text{(Multiply Plane 1 by 3)}
$$

$$
6x + 8y + 4z = 12 \quad \text{(Multiply Plane 2 by 2)}
$$

Now, subtract the second equation from the first:

$$
(6x + 9y + 12z) - (6x + 8y + 4z) = 15 - 12
$$

$$
y + 8z = 3
$$

Solve for \( y \):

$$
y = 3 - 8z
$$

Now, substitute \( y = 3 - 8z \) into one of the original plane equations. Let's use \( 2x + 3y + 4z = 5 \):

$$
2x + 3(3 - 8z) + 4z = 5
$$

$$
2x + 9 - 24z + 4z = 5
$$

$$
2x - 20z = -4
$$

Solve for \( x \):

$$
x = -10z + 2
$$

Thus, we have the parametric equations of the line of intersection:

$$
x = -10z + 2
$$

$$
y = 3 - 8z
$$

$$
z = z
$$

The parametric form of the line of intersection is:

$$
\mathbf{r}(z) = (x, y, z) = (-10z + 2, 3 - 8z, z)
$$

So, the line of intersection can be represented as:

$$
\mathbf{r}(z) = (2, 3, 0) + z(-10, -8, 1)
$$

---

### 5. Write the equation of the plane passing through point \( A(1, 2, 3) \) and parallel to vectors \( \mathbf{v_1} = [1, 0, 1] \) and \( \mathbf{v_2} = [0, 1, -1] \).

The plane passing through a point and parallel to two vectors has a normal vector that is the cross product of the two given vectors. First, compute the cross product of \( \mathbf{v_1} \) and \( \mathbf{v_2} \):

$$
\mathbf{v_1} = (1, 0, 1), \quad \mathbf{v_2} = (0, 1, -1)
$$

The cross product is:

$$
\mathbf{n} = \mathbf{v_1} \times \mathbf{v_2} = 
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
1 & 0 & 1 \\
0 & 1 & -1
\end{vmatrix}
= \hat{i}(0 \cdot (-1) - 1 \cdot 1) - \hat{j}(1 \cdot (-1) - 1 \cdot 0) + \hat{k}(1 \cdot 1 - 0 \cdot 0)
$$

Simplifying:

$$
\mathbf{n} = \hat{i}(-1) - \hat{j}(-1) + \hat{k}(1)
$$

$$
\mathbf{n} = (-1, 1, 1)
$$

The equation of the plane is:

$$
-1(x - 1) + 1(y - 2) + 1(z - 3) = 0
$$

Simplifying:

$$
-x + 1 + y - 2 + z - 3 = 0
$$

$$
-x + y + z = 4
$$

Thus, the equation of the plane is:

$$
-x + y + z = 4
$$

---

### 6. We have the plane \( 2x + 3y + 4z = 5 \). Find an example of a plane parallel and perpendicular to it.

- A plane parallel to \( 2x + 3y + 4z = 5 \) will have the same normal vector, which is \( (2, 3, 4) \). Therefore, the equation of the parallel plane will be of the form:

$$
2x + 3y + 4z = d
$$

For example, if \( d = 10 \), the equation of the parallel plane would be:

$$
2x + 3y + 4z = 10
$$

- A plane perpendicular to \( 2x + 3y + 4z = 5 \) will have a normal vector that is perpendicular to \( (2, 3, 4) \). We can choose any vector orthogonal to \( (2, 3, 4) \). For example, if we take \( (1, -2, 1) \), the equation of the perpendicular plane will be:

$$
1(x - 1) - 2(y + 2) + 1(z - 1) = 0
$$

Expanding:

$$
x - 1 - 2y - 4 + z - 1 = 0
$$

$$
x - 2y + z = 6
$$

Thus, the equation of the perpendicular plane is:

$$
x - 2y + z = 6
$$

---

### 7. We have the plane \( 2x + 3y + 4z = 5 \) and point \( A(1, 2, 3) \). Find the distance from point \( A \) to this plane.

The formula to find the distance from a point \( (x_1, y_1, z_1) \) to a plane \( Ax + By + Cz + D = 0 \) is:

$$
d = \frac{|Ax_1 + By_1 + Cz_1 + D|}{\sqrt{A^2 + B^2 + C^2}}
$$

For the plane \( 2x + 3y + 4z = 5 \), \( A = 2 \), \( B = 3 \), \( C = 4 \), and \( D = -5 \). The point \( A(1, 2, 3) \) has coordinates \( (x_1, y_1, z_1) = (1, 2, 3) \).

Substituting into the formula:

$$
d = \frac{|2(1) + 3(2) + 4(3) - 5|}{\sqrt{2^2 + 3^2 + 4^2}} = \frac{|15|}{\sqrt{29}} = \frac{15}{\sqrt{29}}
$$

Thus, the distance is \( \frac{15}{\sqrt{29}} \).

---

### 8. The plane intersects the coordinate axes at points \( A(2, 0, 0) \), \( B(0, 3, 0) \), and \( C(0, 0, 4) \). Find the equation of the plane.

The equation of the plane can be written as:

$$
\frac{x}{a} + \frac{y}{b} + \frac{z}{c} = 1
$$

The intercepts are \( a = 2 \), \( b = 3 \), and \( c = 4 \), so the equation of the plane is:

$$
\frac{x}{2} + \frac{y}{3} + \frac{z}{4} = 1
$$

Multiplying by 12:

$$
6x + 4y + 3z = 12
$$

Thus, the equation is \( 6x + 4y + 3z = 12 \).

---

### 9. Calculate the angle between the plane \( x + y + z = 1 \) and the plane \( x = 0 \) (i.e., the \( yz \)-plane).

The angle between the planes is given by:

$$
\cos \theta = \frac{\mathbf{n_1} \cdot \mathbf{n_2}}{|\mathbf{n_1}| |\mathbf{n_2}|}
$$

For the planes \( x + y + z = 1 \) and \( x = 0 \), the normal vectors are \( \mathbf{n_1} = (1, 1, 1) \) and \( \mathbf{n_2} = (1, 0, 0) \).

$$
\cos \theta = \frac{1}{\sqrt{3} \cdot 1} = \frac{1}{\sqrt{3}}
$$

Thus, the angle is:

$$
\theta \approx 54.74^\circ
$$

---

### 10. Find the vector perpendicular to the plane \( x + y + z = 1 \).

The vector perpendicular to the plane is simply the normal vector to the plane, which is \( \mathbf{n} = (1, 1, 1) \).

Thus, the vector perpendicular to the plane is \( \mathbf{n} = (1, 1, 1) \).
Problem 7: Finding the angle between vectors a = [3, 1] and b = [2, -1].

Dot Product: $$\mathbf{a} \cdot \mathbf{b} = 3 \cdot 2 + 1 \cdot (-1) = 6 - 1 = 5$$

Magnitudes: $$\| \mathbf{a} \| = \sqrt{3^2 + 1^2} = \sqrt{9 + 1} = \sqrt{10}$$ $$\| \mathbf{b} \| = \sqrt{2^2 + (-1)^2} = \sqrt{4 + 1} = \sqrt{5}$$

Cosine of the Angle: $$\cos \theta = \frac{\mathbf{a} \cdot \mathbf{b}}{\| \mathbf{a} \| \| \mathbf{b} \|} = \frac{5}{\sqrt{10} \cdot \sqrt{5}} = \frac{5}{\sqrt{50}} = \frac{5}{5\sqrt{2}} = \frac{1}{\sqrt{2}} = \frac{\sqrt{2}}{2}$$

Angle: $$\theta = \cos^{-1} \left(\frac{\sqrt{2}}{2}\right) = 45^\circ$$

Problem 8: Finding the volume of the parallelepiped spanned by vectors a = [1, 0, -1], b = [2, 1, 1], and c = [0, -1, 3].

Cross Product of b and c: $$\mathbf{b} \times \mathbf{c} = \left| \begin{matrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & 1 \\ 0 & -1 & 3 \\ \end{matrix} \right| = \mathbf{i} (1 \cdot 3 - 1 \cdot (-1)) - \mathbf{j} (2 \cdot 3 - 1 \cdot 0) + \mathbf{k} (2 \cdot (-1) - 1 \cdot 0)$$

Simplifying: $$\mathbf{b} \times \mathbf{c} = \mathbf{i} (3 + 1) - \mathbf{j} (6) + \mathbf{k} (-2) = \mathbf{i} (4) - \mathbf{j} (6) + \mathbf{k} (-2) = [4, -6, -2]$$

Dot Product of a and (b × c): $$\mathbf{a} \cdot (\mathbf{b} \times \mathbf{c}) = 1 \cdot 4 + 0 \cdot (-6) + (-1) \cdot (-2) = 4 + 0 + 2 = 6$$

Volume: $$V = |6| = 6$$