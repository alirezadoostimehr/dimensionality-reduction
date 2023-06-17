# Problem statement
Show that for every two arbitrary vector spaces $V_1$ and $V_2$ with $B_1$ and $B_2$ as basis respectively, 
if $B_1$ and $B_2$ are homomorphic, then $V_1$ and $V_2$ are homomorphic.

# Solution
Suppose $V_1$ and $V_2$ are two vector spaces with bases $B_1$ and $B_2$ respectively, and let $f:B_1\rightarrow B_2$ be a linear transformation between $B_1$ and $B_2$. We want to show that there exists a linear isomorphism $T:V_1\rightarrow V_2$ that sends basis elements of $V_1$ to basis elements of $V_2$ such that $T(b)=f(b)$ for all $b\in B_1$.

To define $T$, we can use the fact that every vector $v\in V_1$ can be uniquely expressed as a linear combination of basis vectors of $B_1$. Specifically, if $v=a_1b_1+a_2b_2+\cdots+a_nb_n$ where $b_1,b_2,\ldots,b_n$ are basis vectors of $B_1$ and $a_1,a_2,\ldots,a_n\in\mathbb{F}$, then we can define $T(v)=a_1f(b_1)+a_2f(b_2)+\cdots+a_nf(b_n)$.

To show that $T$ is a linear isomorphism, we need to verify that it is a linear transformation, that it is injective, and that it is surjective.

First, we show that $T$ is a linear transformation. Let $v_1,v_2\in V_1$ and $c\in\mathbb{F}$ be arbitrary. Then we have

$$
\begin{aligned}
T(cv_1+v_2) &= T(ca_1b_1+ca_2b_2+\cdots+ca_nb_n+a_1b_1'+a_2b_2'+\cdots+a_mb_m') \\
= caf(b_1)+caf(b_2)+\cdots+caf(b_n)+a_1f(b_1') + a_2f(b_2')+\cdots+a_mf(b_m') \\
= cT(v_1)+T(v_2),
\end{aligned}
$$

where $v_1=a_1b_1+a_2b_2+\cdots+a_nb_n$, $v_2=a_1b_1'+a_2b_2'+\cdots+a_mb_m'$, and $b_1,\ldots,b_n,b_1',\ldots,b_m'$ are basis vectors of $B_1$ and $B_2$ respectively. Therefore, $T$ preserves addition and scalar multiplication, and is therefore a linear transformation.

Next, we show that $T$ is injective. Suppose $T(v_1)=T(v_2)$ for some $v_1,v_2\in V_1$. Then we have

$$
\begin{aligned}
T(v_1)-T(v_2) &= a_1f(b_1)+a_2f(b_2)+\cdots+a_nf(b_n)\\
\qquad -b_1f(b_1)-b_2f(b_2)-\cdots-b_nf(b_n) \\
= (a_1-b_1)f(b_1)+(a_2-b_2)f(b_2)+\cdots+(a_n-b_n)f(b_n) \\
= 0,
\end{aligned}
$$

where $v_1=a_1b_1+a_2b_2+\cdots+a_nb_n$ and $v_2=b_1,b_2,\ldots,b_n$ are basis vectors of $B_1$. Since $B_1$ is a basis of $V_1$, we have $a_1-b_1=a_2-b_2=\cdots=a_n-b_n=0$. Therefore, $v_1=v_2$, and $T$ is injective.

Finally, we show that $T$ is surjective. Let $v'\in V_2$ be arbitrary. Since $B_2$ is a basis of $V_2$, we can write $v'$ as a linear combination of basis vectors of $B_2$. Specifically, if $v'=c_1b_1+c_2b_2+\cdots+c_mb_m$ where $b_1,b_2,\ldots,b_m$ are basis vectors of $B_2$ and $c_1,c_2,\ldots,c_m\in\mathbb{F}$, then we can define $v=c_1f^{-1}(b_1)+c_2f^{-1}(b_2)+\cdots+c_mf^{-1}(b_m)$, where $f^{-1}$ is the inverse of $f$ under the basis $B_1$. By construction, we have $T(v)=v'$, since

$$
\begin{aligned}
T(v) &= T(c_1f^{-1}(b_1)+c_2f^{-1}(b_2)+\cdots+c_mf^{-1}(b_m)) \\
= c_1f(f^{-1}(b_1))+c_2f(f^{-1}(b_2))+\cdots+c_mf(f^{-1}(b_m)) \\
= c_1b_1+c_2b_2+\cdots+c_mb_m \\
= v'.
\end{aligned}
$$

Therefore, $T$ is surjective.

Since $T$ is a bijective linear transformation, it is a linear isomorphism. Therefore, $V_1$ and $V_2$ are isomorphic as vector spaces, and $B_1$ and $B_2$ are isomorphic as bases.
