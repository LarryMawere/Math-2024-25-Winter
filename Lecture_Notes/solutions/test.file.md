# Solution 1: Basic Operations on Matrices

## 1.1 Addition and Subtraction

1. $A + B$:
   $$
   A + B = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} + \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}
   = \begin{bmatrix} 1+5 & 2+6 \\ 3+7 & 4+8 \end{bmatrix}
   = \begin{bmatrix} 6 & 8 \\ 10 & 12 \end{bmatrix}.
   $$

2. $B - A$:
   $$
   B - A = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix} - \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}
   = \begin{bmatrix} 5-1 & 6-2 \\ 7-3 & 8-4 \end{bmatrix}
   = \begin{bmatrix} 4 & 4 \\ 4 & 4 \end{bmatrix}.
   $$

3. $A + C$:
   $$
   A + C = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} + \begin{bmatrix} -1 & 2 \\ 3 & 0 \end{bmatrix}
   = \begin{bmatrix} 1+(-1) & 2+2 \\ 3+3 & 4+0 \end{bmatrix}
   = \begin{bmatrix} 0 & 4 \\ 6 & 4 \end{bmatrix}.
   $$

4. $D + E$:
   $$
   D + E = \begin{bmatrix} -1 & 2 & 3 \\ 4 & 0 & 6 \end{bmatrix} + \begin{bmatrix} 1 & 2 & 4 \\ 5 & 7 & 8 \end{bmatrix}
   = \begin{bmatrix} -1+1 & 2+2 & 3+4 \\ 4+5 & 0+7 & 6+8 \end{bmatrix}
   = \begin{bmatrix} 0 & 4 & 7 \\ 9 & 7 & 14 \end{bmatrix}.
   $$

## 1.2 Scalar Multiplication

1. $2A$:
   $$
   2A = 2 \cdot \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}
   = \begin{bmatrix} 2 \cdot 1 & 2 \cdot 2 \\ 2 \cdot 3 & 2 \cdot 4 \end{bmatrix}
   = \begin{bmatrix} 2 & 4 \\ 6 & 8 \end{bmatrix}.
   $$

2. $-3C$:
   $$
   -3C = -3 \cdot \begin{bmatrix} -1 & 2 \\ 3 & 0 \end{bmatrix}
   = \begin{bmatrix} -3 \cdot (-1) & -3 \cdot 2 \\ -3 \cdot 3 & -3 \cdot 0 \end{bmatrix}
   = \begin{bmatrix} 3 & -6 \\ -9 & 0 \end{bmatrix}.
   $$

3. $4D$:
   $$
   4D = 4 \cdot \begin{bmatrix} -1 & 2 & 3 \\ 4 & 0 & 6 \end{bmatrix}
   = \begin{bmatrix} 4 \cdot (-1) & 4 \cdot 2 & 4 \cdot 3 \\ 4 \cdot 4 & 4 \cdot 0 & 4 \cdot 6 \end{bmatrix}
   = \begin{bmatrix} -4 & 8 & 12 \\ 16 & 0 & 24 \end{bmatrix}.
   $$

## 1.3 Matrix Multiplication

1. $AB$:
   $$
   A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}
   $$
   $$
   AB = \begin{bmatrix} 1 \cdot 5 + 2 \cdot 7 & 1 \cdot 6 + 2 \cdot 8 \\ 3 \cdot 5 + 4 \cdot 7 & 3 \cdot 6 + 4 \cdot 8 \end{bmatrix}
   = \begin{bmatrix} 19 & 22 \\ 43 & 50 \end{bmatrix}.
   $$

2. $AD$:
   $$
   A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad D = \begin{bmatrix} -1 & 2 & 3 \\ 4 & 0 & 6 \end{bmatrix}
   $$
   $$
   AD = \begin{bmatrix} 1 \cdot (-1) + 2 \cdot 4 & 1 \cdot 2 + 2 \cdot 0 & 1 \cdot 3 + 2 \cdot 6 \\ 
   3 \cdot (-1) + 4 \cdot 4 & 3 \cdot 2 + 4 \cdot 0 & 3 \cdot 3 + 4 \cdot 6 \end{bmatrix}
   = \begin{bmatrix} 7 & 2 & 15 \\ 13 & 6 & 33 \end{bmatrix}.
   $$

3. $DE$:
   $$
   D = \begin{bmatrix} -1 & 2 & 3 \\ 4 & 0 & 6 \end{bmatrix}, \quad E = \begin{bmatrix} 1 & 2 & 4 \\ 5 & 7 & 8 \end{bmatrix}
   $$
   Multiplication is not possible as the number of columns in $D$ is 3, and the number of rows in $E$ is 2.
