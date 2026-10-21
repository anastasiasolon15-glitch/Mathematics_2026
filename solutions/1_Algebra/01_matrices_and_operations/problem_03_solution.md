# Exercise 3. When Can Matrices Be Multiplied?

## Question

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

### Steps

The product $XY$ of an $m\times n$ matrix $X$ and a $p\times q$ matrix $Y$ is defined if and only if $n=p$ (the number of columns of $X$ equals the number of rows of $Y$). The result then has size $m\times q$.

| Product | Sizes | Condition | Defined | Size of result |
|---|---|---|---|---|
| $AB$ | $2\times3$, $3\times4$ | $3=3$ | yes | $2\times4$ |
| $BA$ | $3\times4$, $2\times3$ | $4\neq2$ | no | none |
| $BC$ | $3\times4$, $4\times2$ | $4=4$ | yes | $3\times2$ |
| $CB$ | $4\times2$, $3\times4$ | $2\neq3$ | no | none |
| $AC$ | $2\times3$, $4\times2$ | $3\neq4$ | no | none |
| $CA$ | $4\times2$, $2\times3$ | $2=2$ | yes | $4\times3$ |
| $AD$ | $2\times3$, $2\times2$ | $3\neq2$ | no | none |
| $DA$ | $2\times2$, $2\times3$ | $2=2$ | yes | $2\times3$ |

### Result

The products $AB$, $BC$, $CA$, $DA$ are defined, with sizes $2\times4$, $3\times2$, $4\times3$, $2\times3$ respectively. The products $BA$, $CB$, $AC$, $AD$ are not defined.

### Method

Each entry of $XY$ is a dot product of a row of $X$ with a column of $Y$. A dot product requires vectors of equal length, and the row length of $X$ is its number of columns, while the column length of $Y$ is its number of rows.

### Verification

The pair $AB$ is defined while $BA$ is not, which shows that the order of factors matters even for the existence of the product. Chains are consistent: $AB$ has size $2\times4$ and $C$ has size $4\times2$, so $(AB)C$ is defined with size $2\times2$. The same size follows from $A(BC)$, where $BC$ is $3\times2$ and $A$ is $2\times3$.
