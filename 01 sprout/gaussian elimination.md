# gaussian elimination
---
Topics: #math
Created: 2022-11-25 09:19:58

---

It is also known as the row reduction method and allows us to solve some linear set of equations

This is used heavily to find the [[eigen vector]] from a matrix

$$
\begin{bmatrix}
    x_{11} & x_{12} & x_{13} & \dots  & x_{1n} \\
    x_{21} & x_{22} & x_{23} & \dots  & x_{2n} \\
    \vdots & \vdots & \vdots & \ddots & \vdots \\
    x_{d1} & x_{d2} & x_{d3} & \dots  & x_{dn}
\end{bmatrix}
$$

## Example

$$
\begin{bmatrix}
	1 & 1 & 1 \\
	1 & 2 & 3 \\
	2 & 3 & 4 \\
\end{bmatrix}
\begin{bmatrix}
	x \\
	y \\
	z \\
\end{bmatrix}
=
\begin{bmatrix}
2 \\
5 \\
11 \\
\end{bmatrix}
$$

This is our initial set of equations. We can convert this into the augmented matrix form

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
1 & 2 & 3 & 5 \\
2 & 3 & 4 & 11 \\
\end{array}
\right]
\Rightarrow
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
0 & 1 & 2 & 3 \\
2 & 3 & 4 & 11 \\
\end{array}
\right]
$$

# References
