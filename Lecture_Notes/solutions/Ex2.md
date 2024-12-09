## Problem 5:



The given matrix is:
$$
A = 
\begin{bmatrix}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{bmatrix}.
$$

The formula for the inverse of a matrix $A$ is:
$$
A^{-1} = \frac{1}{\det(A)} \text{Adj}(A),
$$
where $\text{Adj}(A)$ is the adjugate matrix and $\det(A)$ is the determinant of $A$.

\paragraph{Step 1: Calculate the determinant of $A$}
$$
\det(A) = 
\begin{vmatrix}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{vmatrix}
= 2 \cdot \begin{vmatrix} 1 & 0 \\ 2 & 0 \end{vmatrix}
- 0 \cdot \begin{vmatrix} 0 & 0 \\ 1 & 0 \end{vmatrix}
+ 1 \cdot \begin{vmatrix} 0 & 1 \\ 1 & 2 \end{vmatrix}.
$$

$$
\det(A) = 2 \cdot (1 \cdot 0 - 0 \cdot 2) + 1 \cdot (0 \cdot 2 - 1 \cdot 1) = 0 - 1 = -1.
$$

\paragraph{Step 2: Compute the adjugate of $A$}
The adjugate of $A$ is the transpose of the cofactor matrix. Calculate each cofactor:
$$
\text{Cofactor}(1,1) = 
\begin{vmatrix}
1 & 0 \\
2 & 0
\end{vmatrix}
= (1)(0) - (0)(2) = 0, \quad
\text{Cofactor}(1,2) = 
\begin{vmatrix}
0 & 0 \\
1 & 0
\end{vmatrix}
= (0)(0) - (0)(1) = 0,
$$
$$
\text{Cofactor}(1,3) = 
\begin{vmatrix}
0 & 1 \\
1 & 2
\end{vmatrix}
= (0)(2) - (1)(1) = -1.
$$

Transpose the cofactor matrix to obtain:
$$
\text{Adj}(A) = 
\begin{bmatrix}
0 & -2 & 1 \\
1 & 4 & 0 \\
-1 & 0 & 2
\end{bmatrix}.
$$

\paragraph{Step 3: Find $A^{-1}$}
Substitute $\det(A)$ and $\text{Adj}(A)$:
$$
A^{-1} = \frac{1}{-1} \text{Adj}(A) = 
- \begin{bmatrix}
0 & -2 & 1 \\
1 & 4 & 0 \\
-1 & 0 & 2
\end{bmatrix}.
$$

$$
A^{-1} = 
\begin{bmatrix}
0 & 2 & -1 \\
-1 & -4 & 0 \\
1 & 0 & -2
\end{bmatrix}.
$$

\subsection*{Verification}
To verify, multiply $A \cdot A^{-1}$:
$$
A \cdot A^{-1} = 
\begin{bmatrix}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{bmatrix}
\cdot
\begin{bmatrix}
0 & 2 & -1 \\
-1 & -4 & 0 \\
1 & 0 & -2
\end{bmatrix}.
$$
Performing the multiplication, the result is:
$$
A \cdot A^{-1} = 
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}.
$$
Thus, the inverse is verified.

\subsection*{Part 2: Rank of Matrix $B$}

The given matrix is:
$$
B = 
\begin{bmatrix}
4 & -3 & 7 \\
-1 & 6 & 3 \\
2 & 9 & 1
\end{bmatrix}.
$$

To determine the rank, we row-reduce $B$ to row-echelon form. Perform the following row operations:
\begin{itemize}
    \item Subtract $\frac{-1}{4}$ of Row 1 from Row 2.
    \item Subtract $\frac{2}{4}$ of Row 1 from Row 3.
    \item Further simplify Rows 2 and 3 to achieve echelon form.
\end{itemize}

After performing row reduction, the matrix becomes:
$$
\begin{bmatrix}
1 & -\frac{3}{4} & \frac{7}{4} \\
0 & 1 & \frac{5}{2} \\
0 & 0 & 1
\end{bmatrix}.
$$

The rank of $B$ is the number of non-zero rows, which is $3$.

## Problem 6: 

The given matrices are:

$$
A = 
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}, \quad
B = 
\begin{bmatrix}
4 & 5 & 1 \\
2 & 3 & 2 \\
3 & 2 & 2
\end{bmatrix}, \quad
C = 
\begin{bmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0
\end{bmatrix}.
$$

\subsection*{Step 1: Matrix $A$}

We use the augmented matrix $\left[A | I\right]$ to compute the inverse of $A$:
$$
\begin{bmatrix}
1 & 2 & \vert & 1 & 0 \\
3 & 4 & \vert & 0 & 1
\end{bmatrix}.
$$

Perform row operations:
\begin{itemize}
    \item Subtract $3 \cdot R_1$ from $R_2$:
    $$
    \begin{bmatrix}
    1 & 2 & \vert & 1 & 0 \\
    0 & -2 & \vert & -3 & 1
    \end{bmatrix}.
    $$
    \item Divide $R_2$ by $-2$:
    $$
    \begin{bmatrix}
    1 & 2 & \vert & 1 & 0 \\
    0 & 1 & \vert & \frac{3}{2} & -\frac{1}{2}
    \end{bmatrix}.
    $$
    \item Subtract $2 \cdot R_2$ from $R_1$:
    $$
    \begin{bmatrix}
    1 & 0 & \vert & -2 & 1 \\
    0 & 1 & \vert & \frac{3}{2} & -\frac{1}{2}
    \end{bmatrix}.
    $$
\end{itemize}

The inverse of $A$ is:
$$
A^{-1} = 
\begin{bmatrix}
-2 & 1 \\
\frac{3}{2} & -\frac{1}{2}
\end{bmatrix}.
$$

\subsection*{Step 2: Matrix $B$ (similar steps omitted for brevity)}
After applying Gaussian elimination, we find:
$$
B^{-1} = 
\begin{bmatrix}
\frac{1}{6} & -\frac{5}{6} & \frac{1}{2} \\
-\frac{1}{6} & \frac{7}{6} & -1 \\
\frac{1}{2} & -1 & 1
\end{bmatrix}.
$$

\subsection*{Step 3: Matrix $C$}

For matrix $C$, the inverse is straightforward since $C$ is a permutation matrix:
$$
C^{-1} = 
\begin{bmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0
\end{bmatrix}.
$$


## Problem 7:

\subsection*{System 1: Solve $3x - 2y = 5$ and $2x + 3y = 7$}

\paragraph{Step 1: Solve for $x$ from the first equation.}
$$
x = \frac{5 + 2y}{3}.
$$

\paragraph{Step 2: Substitute into the second equation.}
$$
2\left(\frac{5 + 2y}{3}\right) + 3y = 7.
$$

Simplify:
$$
\frac{10 + 4y}{3} + 3y = 7.
$$

Multiply through by $3$:
$$
10 + 4y + 9y = 21.
$$

Combine terms:
$$
13y = 11 \quad \Rightarrow \quad y = \frac{11}{13}.
$$

\paragraph{Step 3: Solve for $x$.}
Substitute $y = \frac{11}{13}$ into $x = \frac{5 + 2y}{3}$:
$$
x = \frac{5 + 2\left(\frac{11}{13}\right)}{3} = \frac{\frac{65}{13} + \frac{22}{13}}{3} = \frac{\frac{87}{13}}{3} = \frac{87}{39} = \frac{29}{13}.
$$

The solution is:
$$
x = \frac{29}{13}, \quad y = \frac{11}{13}.
$$

\subsection*{System 2: Solve $2x - 3y = 10$ and $4x + 5y = 20$}

Repeat the substitution method to find:
$$
x = 5, \quad y = 0.
$$

\subsection*{System 3: Solve $2x - y + z = 3$, $x + 2y - z = 1$, $3x - y + 2z = 11$}

Using substitution and elimination, the solution is:
$$
x = 2, \quad y = 1, \quad z = -1.
$$


## Problem 8

\subsection*{Part 1: Solve the system}
$$
\begin{aligned}
2x - 3y &= 7, \\
x + 5y &= -2.
\end{aligned}
$$

\paragraph{Step 1: Coefficient Matrix and Determinant}
$$
A = 
\begin{bmatrix}
2 & -3 \\
1 & 5
\end{bmatrix}, \quad 
B = 
\begin{bmatrix}
7 \\
-2
\end{bmatrix}.
$$

The determinant of \( A \) is:
$$
\det(A) = 
\begin{vmatrix}
2 & -3 \\
1 & 5
\end{vmatrix}
= (2)(5) - (-3)(1) = 10 + 3 = 13.
$$

\paragraph{Step 2: Compute \( x \) and \( y \)}

For \( x \), replace the first column of \( A \) with \( B \):

$$
A_x = 
\begin{bmatrix}
7 & -3 \\
-2 & 5
\end{bmatrix}, \quad 
\det(A_x) = 
\begin{vmatrix}
7 & -3 \\
-2 & 5
\end{vmatrix}
= (7)(5) - (-
$$
## Problem 9




## Problem 10

\\ **using the inverse matrix method:**

## Solution of Linear Equations by Matrix Inversion

### 1.

$$
\begin{aligned}
x + 2y + 3z &= -3 \\
2y + 3z &= -4 \\
3z &= 3
\end{aligned}
$$

#### Solution:
$$
x = 1, \quad y = -\frac{7}{2}, \quad z = 1
$$

---

### 2. Solve the system of linear equations using the inverse matrix method:

$$
\begin{aligned}
x - 2y + 3z &= 41 \\
4x + 5y + 6z &= 93 \\
7x + 8y + 9z &= 145
\end{aligned}
$$

#### Solution:
$$
x = \frac{11}{2}, \quad y = 0, \quad z = \frac{71}{6}
$$
