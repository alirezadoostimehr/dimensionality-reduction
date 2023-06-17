# Problem statement
Show that $V$ is isomorphic to $C$.

# Solution
If $C$ is the field of complex numbers:

Let $V$ be a vector space over the field $\mathbb{R}$, and let $C$ be the field of complex numbers. We want to show that $V$ is isomorphic to $C$.

Since $C$ is a field, it is a one-dimensional vector space over itself. Therefore, any non-zero complex number can serve as a basis for $C$. Let us choose the complex number $1$ as the basis for $C$.

Since $V$ is a vector space, it has a basis $B={v_1,v_2,\ldots,v_n}$. Let $f:V\rightarrow C$ be the linear transformation defined by $f(v_1)=1$ and $f(v_i)=0$ for $i=2,3,\ldots,n$. In other words, $f$ maps the first basis vector of $V$ to the basis vector $1$ of $C$, and maps all other basis vectors of $V$ to $0$.

We claim that $f$ is an isomorphism between $V$ and $C$. First, we show that $f$ is linear. Let $u,v\in V$ be arbitrary vectors, and let $a,b\in\mathbb{R}$ be arbitrary scalars. Then we have

$$
\begin{aligned}
f(au+bv) &= f(av_1+bv_2+\cdots+bv_n) \\
= af(v_1)+bf(v_2)+\cdots+bf(v_n) \\
= a\cdot 1+0+\cdots+0 \\
= a,
\end{aligned}
$$

where we have used the fact that $f(v_i)=0$ for $i=2,3,\ldots,n$. Therefore, $f$ preserves addition and scalar multiplication, and is hence linear.

Next, we show that $f$ is injective. Suppose $f(u)=f(v)$ for some $u,v\in V$. Then we have $f(u)=a$ and $f(v)=a$ for some $a\in\mathbb{R}$. Since $f(u)=a$, we must have $u$ equal to $v_1$ (the first basis vector of $V$), since $f(v_1)=1$ and $f(v_i)=0$ for $i=2,3,\ldots,n$. Similarly, since $f(v)=a$, we must have $v$ equal to $v_1$. Therefore, $u=v$, and hence $f$ is injective.

Finally, we show that $f$ is surjective. Let $a\in C$ be an arbitrary complex number. Then we have $a=b+ci$ for some $b,c\in\mathbb{R}$. Let $v=bv_1+cv_2$. Then we have

$$
f(v) = bf(v_1)+cf(v_2) = b = Re(a),
$$

where $Re(a)$ denotes the real part of the complex number $a$. Therefore, for any $a\in C$, there exists a $v\in V$ such that $f(v)=a$, and hence $f$ is surjective.

Since $f$ is both linear and bijective, it is an isomorphism between $V$ and $C$. Therefore, $V$ is isomorphic to $C$.
