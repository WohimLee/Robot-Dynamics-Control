&emsp;
# Rotational Transformations

<div align=center>
    <img src="imgs/2.6.png" width=300>
    <h4>Figure 2.6: Coordinate frame attached to a rigid body<h>
</div>
&emsp;

Figure 2.6 shows a rigid object $S$ to which a coordinate frame $o_1-x_1-y_1-z_1$ is attached. Given the coordinates $p1$ of the point $p$ (i.e., given the coordinates of p with respect to the frame o1x1y1z1), we wish to determine the coordinates of $p$ relative to a fixed reference frame $o_0-x_0-y_0-z_0$.

The coordinates $p^1 = (u, v, w)^t$ satisfy the equation

$$p = ux_1 + vy_1 +wz_1 \tag{2.22}$$

In a similar way, we can obtain an expression for the coordinates $p_0$ by projecting the point $p$ onto the coordinate axes of the frame $o_0-x_0-y_0-z_0$, giving

$$p^0 = \begin{bmatrix}p\cdot x_0 \\ p\cdot y_0 \\ p\cdot z_0\end{bmatrix} \tag{2.23}$$

Combining these two equations we obtain

$$p^0 = \begin{bmatrix}(ux_1 + vy_1 + wz_1)\cdot x_0 \\
(ux_1 + vy_1 + wz_1)\cdot y_0 \\
(ux_1 + vy_1 + wz_1)\cdot z_0
\end{bmatrix} \tag{2.24} $$

$$\qquad\quad\ \ \ = \begin{bmatrix}ux_1 \cdot x_0 + vy_1\cdot x_0 + wz_1 \cdot x_0 \\
ux_1 \cdot y_0 + vy_1\cdot y_0 + wz_1 \cdot y_0 \\
ux_1 \cdot z_0 + vy_1\cdot z_0 + wz_1 \cdot z_0 
\end{bmatrix}\tag{2.25}$$

$$\qquad\quad\ \ \ = \begin{bmatrix}x_1 \cdot x_0 & y_1\cdot x_0 & z_1\cdot x_0 \\ 
x_1 \cdot y_0 & y_1\cdot y_0 & z_1\cdot y_0 \\ 
x_1 \cdot z_0 & y_1\cdot z_0 & z_1\cdot z_0 
\end{bmatrix}\begin{bmatrix}u \\ v \\ w\end{bmatrix} \tag{2.26}$$

But the matrix in this final equation is merely the rotation matrix $R^0_1$, which leads to

$$p^0 = R^0_1p^1$$



