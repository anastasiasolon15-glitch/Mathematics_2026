# Exercise 15: Complete Classification of a Line Relative to a Plane

Let

$$
L:p+tv,\qquad \Pi:n\cdot x=d.
$$

Substituting $p+tv$ into the plane gives

$$
(n\cdot v)t=n\cdot p-d.
$$

The classifications are:

- **One intersection point:** $n\cdot v\neq0$. Then

$$
t=\frac{d-n\cdot p}{n\cdot v}.
$$

- **Parallel with no common points:** $n\cdot v=0$ and $n\cdot p-d\neq0$.
- **Line contained in the plane:** $n\cdot v=0$ and $n\cdot p-d=0$.

## Numerical examples

### One intersection

Let

$$
p=(0,0,0),\quad v=(1,0,0),
$$

and let the plane be $x=2$. Then $n=(1,0,0)$, so $n\cdot v=1\neq0$, and the intersection is $(2,0,0)$.

### Parallel with no common point

Keep $v=(0,1,0)$ and take $p=(0,0,0)$ with the plane $x=2$. Then $n\cdot v=0$, but $n\cdot p-d=-2\neq0$. The line has coordinates $(0,t,0)$ and never reaches $x=2$.

### Contained in the plane

Let

$$
p=(0,0,0),\quad v=(0,1,0),
$$

and take the plane $x=0$. Here $n\cdot v=0$ and $n\cdot p-d=0$, so every point $(0,t,0)$ lies in the plane.
