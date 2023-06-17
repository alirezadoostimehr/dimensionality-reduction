# Problem statement
Consider the vector space $C$ in previous section. Show that $V$ is isomorphic to $C$.

# Solution

To show that $V$ is isomorphic to $C$, we need to find a bijective linear transformation $T:V\rightarrow C$ that preserves the linear structure 
(i.e., that satisfies $T(\lambda\mathbf{u}+\mu\mathbf{v})=\lambda T(\mathbf{u})+\mu T(\mathbf{v})$ for all $\mathbf{u},\mathbf{v}\in V$ 
and all $\lambda,\mu\in\mathbb{R}$).

Let $T:V\rightarrow C$ be the linear transformation defined by $T(a,b) = (a,b,1)$.

First, we show that $T$ is bijective. 

To see that $T$ is injective, suppose that $T(\mathbf{u})=T(\mathbf{v})$ for some $\mathbf{u},\mathbf{v}\in V$. 
Then we have $(u_1,u_2,1) = T(\mathbf{u}) = T(\mathbf{v}) = (v_1,v_2,1)$. Therefore, we must have $u_1=v_1$, $u_2=v_2$, and $1=1$. 
Hence, $\mathbf{u}=\mathbf{v}$, and $T$ is injective.

To see that $T$ is surjective, let $(a,b,1)\in C$ be an arbitrary point. Since $C$ is a line in $\mathbb{P}^2$, 
we can choose a point $(c,d,e)\in\mathbb{R}^3$ that is not on the line $C$ and that satisfies $\alpha c + \beta d = \gamma e$, 
where $\alpha,\beta,\gamma$ are the coefficients in the equation of $C$. Then the line passing through $(a,b,1)$ and $(c,d,e)$ intersects $C$ in exactly one point, 
which we can compute as the projection of $(c,d,e)$ onto $C$. 
Let $T(\mathbf{u})$ be this projection, where $\mathbf{u}=(a,b)\in V$. Then $T$ is surjective.

Next, we show that $T$ preserves the linear structure. Let $\mathbf{u},\mathbf{v}\in V$ and let $\lambda,\mu\in R$ be arbitrary. 
Then we have $T(\lambda u+\mu v)$ = $T(\lambda u_1+\mu v_1,\lambda u_2+\mu v_2)$ = 
$(\lambda u_1+\mu v_1,\lambda u_2+\mu v_2,1)$ = $\lambda(u_1,u_2,1) + \mu(v_1,v_2,1)$ = $\lambda T(u) + \mu T(v)$. 
Therefore, $T$ preserves the linear structure.

Since $T$ is bijective and preserves the linear structure, it is an isomorphism between $V$ and $C$. Therefore, $V$ is isomorphic to $C$.
