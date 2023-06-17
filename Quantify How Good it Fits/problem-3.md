# Problem statement
Find a line $C^\*$ minimizing the sum $S$, using only rotation about the origin.

# Solution
To find a line $C^\*$ that minimizes the sum $S$, we want to rotate the coordinate system so that the line $C^\*$ is aligned with the $y$-axis. We can achieve this by rotating the points in the original coordinate system by an angle $\theta$ about the origin, where $\theta$ is chosen so that the line $C$ is rotated to the $y$-axis.

To find the value of $\theta$, we note that the slope of the line $C$ is given by $-\frac{a}{b}$, so the angle between the line $C$ and the $y$-axis is given by $\theta = \tan^{-1}\left(\frac{a}{b}\right)$. We can then perform the rotation by multiplying each point in the original coordinate system by the matrix

$$R = \begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}$$

This rotates each point $(x_i,y_i)$ to the new point $(x'_i,y'_i)$ given by:

$$\begin{pmatrix}
x'_i \
y'_i
\end{pmatrix} = R\begin{pmatrix}
x_i \
y_i
\end{pmatrix}$$

Note that the coefficients of the line $C$ in the new coordinate system are given by $a'=0$ and $b'=1$, since the line is aligned with the $y$-axis. Therefore, the equation of the line $C^\*$ in the new coordinate system is simply $y'=c'$, where $c'$ is the $y$-intercept of the line $C$ in the new coordinate system.

To compute $c'$, we note that the equation of the line $C$ in the original coordinate system is given by $ax+by+c=0$, so the $y$-intercept $c$ is given by $c=-\frac{a}{b}x-\frac{c}{b}$. Substituting $a'=0$ and $b'=1$, we obtain:

$$c' = -\frac{a}{b}\cdot 0 - \frac{c}{b} = -\frac{c}{b}$$

Therefore, the equation of the line $C^\*$ in the new coordinate system is $y'=-\frac{c}{b}$.

We can now compute the sum $S$ in the new coordinate system using the formula derived in the previous question:

$$S = \frac{1}{\sqrt{a'^2+b'^2}} \sum_{i=1}^n |c'-y'i| = \frac{1}{\sqrt{1}} \sum{i=1}^n |c'-y'i| = \sum{i=1}^n |c'+\frac{a}{b}x_i-y_i|$$

Note that $c'$ is a constant that does not depend on $i$, so we can factor it out of the sum:

$$S = \sum_{i=1}^n \left|-\frac{a}{b}x_i+\frac{c}{b}-y_i\right|$$

This expression can be minimized by choosing the value of $c$ that minimizes the sum of the absolute differences $|-\frac{a}{b}x_i+\frac{c}{b}-y_i|$. This can be done using the median, which is the value of $c$ that minimizes the sum of the absolute differences when the sum is evaluated over the median of the $y$-coordinates of the points.

Therefore, the line $C^\*$ that minimizes the sum $S$ is obtained by rotating the coordinate system by an angle $\theta=\tan^{-1}\left(\frac{a}{b}\right)$ and setting the $y$-intercept of the line $C^\*$ to be the median of the $y$-coordinates of the points.
