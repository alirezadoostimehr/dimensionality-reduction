# Problem statement

Let $d_C(X_i)$ be the distance between point $X_i$ and line $C$. Find $S$ = $\Sigma_{1}^n d_c(X_i)$.

# Solution
Recall that the equation of the line $C$ in homogeneous coordinates is given by $ax+by+c=0$, where $(a,b,c)$ are the coefficients of the line. Also recall that the distance between a point $(x_i,y_i)$ and a line $ax+by+c=0$ is given by the formula:

$$d_C(X_i) = \frac{|ax_i+by_i+c|}{\sqrt{a^2+b^2}}$$

Using this formula, we can compute the distance $d_C(X_i)$ between each point $X_i=(x_i,y_i)$ and the line $C$. Then, we can add up all these distances to obtain the sum $S$:

$$S = \Sigma_{i=1}^n d_C(X_i) = \Sigma_{i=1}^n \frac{|ax_i+by_i+c|}{\sqrt{a^2+b^2}}$$

Note that the denominator $\sqrt{a^2+b^2}$ is constant with respect to $i$, so we can factor it out of the sum:

$$S = \frac{1}{\sqrt{a^2+b^2}} \Sigma_{i=1}^n |ax_i+by_i+c|$$
