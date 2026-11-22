# Exercise 13: Closest Point on a Plane

The plane is

$$
x+2y+2z=4
$$

with normal $n=(1,2,2)$. The closest point to $P=(3,0,0)$ is its orthogonal projection onto the plane.

A perpendicular line is

$$
(x,y,z)=P+t(1,2,2).
$$

Substitution into the plane gives

$$
(3+t)+2(2t)+2(2t)=4,
$$

so

$$
3+9t=4,\qquad t=\frac19.
$$

The closest point is therefore

$$
Q=\left(3+\frac19,\frac29,\frac29\right)
=\left(\frac{28}{9},\frac29,\frac29\right).
$$

The signed plane value at $P$ is $3-4=-1$, so the distance is

$$
\frac{|3-4|}{\sqrt{1^2+2^2+2^2}}=\frac13.
$$

Finally,

$$
P-Q=\left(-\frac19,-\frac29,-\frac29\right),
$$

which is a scalar multiple of $n=(1,2,2)$. Thus $PQ$ is perpendicular to the plane.
