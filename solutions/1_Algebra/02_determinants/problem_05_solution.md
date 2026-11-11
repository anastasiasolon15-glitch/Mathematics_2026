## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

### Method

We reduce $A$ to an upper triangular matrix, whose determinant is the product of its diagonal entries. We use only operations of the type "add a multiple of one row to another row". These operations do not change the determinant, so no correction factor is needed.

### Step 1: $R_2\leftarrow R_2-2R_1$

This eliminates the entry below the first pivot in row 2. The determinant does **not** change.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

### Step 2: $R_3\leftarrow R_3+R_1$

This eliminates the entry below the first pivot in row 3. The determinant does **not** change.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

### Step 3: $R_3\leftarrow R_3+2R_2$

This eliminates the entry below the second pivot. The determinant does **not** change.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

### Computing the determinant

The final matrix is upper triangular, and all three operations preserved the determinant. Hence

$$
\det A = 1\cdot(-3)\cdot(-7)=21.
$$

### Check

Sarrus' rule gives

$$
\det A=(1\cdot1\cdot2+2\cdot0\cdot(-1)+3\cdot2\cdot4)-(3\cdot1\cdot(-1)+1\cdot0\cdot4+2\cdot2\cdot2)=26-5=21.
$$

### Answer

$$
\det A = 21.
$$
