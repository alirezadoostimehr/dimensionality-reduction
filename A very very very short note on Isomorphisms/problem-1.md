# Problem statement
Show that $V$ is isomorphic to $K^n$ where $dim(V) = n$.

*Hypotheses: V is a finite dimensional space over the field K.*

# Solution

 To begin with, it is essential to establish that $K^n$ is a vector space, as this is a fundamental requirement for demonstrating the isomorphism to $V$.

 $\textbf{Proof that}$ &nbsp; $K^n$ &nbsp; $\textbf{is a vector space:}$

Assume $K$ is a field and $K^n$ is the set of all $n$-tuples of elements in $K$. Then, $K^n$ is a vector space over $K$ under the operations of coordinate-wise addition and scalar multiplication.

To show that $K^n$ satisfies the axioms of a vector space, we need to verify each of the ten axioms listed below.

1. Closure under addition: For any vectors $\mathbf{u}, \mathbf{v} \in K^n$, $\mathbf{u}+\mathbf{v}$ is also in $K^n$.
   - This is true by definition of $K^n$ as the set of all $n$-tuples of elements in $K$.

2. Commutativity of addition: For any vectors $\mathbf{u}, \mathbf{v} \in K^n$, $\mathbf{u}+\mathbf{v}=\mathbf{v}+\mathbf{u}$.
   - This is true because coordinate-wise addition is commutative.

3. Associativity of addition: For any vectors $\mathbf{u}, \mathbf{v}, \mathbf{w} \in K^n$, $\mathbf{u}+(\mathbf{v}+\mathbf{w})=(\mathbf{u}+\mathbf{v})+\mathbf{w}$.
   - This is true because coordinate-wise addition is associative.

4. Identity element of addition: There exists a vector $\mathbf{0} \in K^n$ such that for any vector $\mathbf{u} \in K^n$, $\mathbf{u}+\mathbf{0}=\mathbf{u}$.
   - This is true because the $n$-tuple of zeros $(0, 0, ..., 0)$ serves as the additive identity element.

5. Inverse elements of addition: For any vector $\mathbf{u} \in K^n$, there exists a vector $-\mathbf{u} \in K^n$ such that $\mathbf{u}+(-\mathbf{u})=\mathbf{0}$.
   - This is true because for any $n$-tuple $\mathbf{u} = (u_1, u_2, ..., u_n)$, its additive inverse $-\mathbf{u}$ is given by $(-u_1, -u_2, ..., -u_n)$.

6. Closure under scalar multiplication: For any scalar $a \in K$ and any vector $\mathbf{u} \in K^n$, the product $a\mathbf{u}$ is also in $K^n$.
   - This is true by definition of scalar multiplication as coordinate-wise multiplication of a scalar and a vector.

7. Distributivity of scalar multiplication over vector addition: For any scalar $a \in K$ and any vectors $\mathbf{u},\mathbf{v} \in K^n$, $a(\mathbf{u}+\mathbf{v})=a\mathbf{u}+a\mathbf{v}$.
   - This is true because scalar multiplication and coordinate-wise addition distribute over each other.

8. Distributivity of scalar multiplication over scalar addition: For any scalars $a, b \in K$ and any vector $\mathbf{u} \in K^n$, $(a+b)\mathbf{u}=a\mathbf{u}+b\mathbf{u}$.
   - This is true because scalar multiplication distributes over scalar addition and vice versa.

9. Associativity of scalar multiplication: For any scalars $a, b \in K$ and any vector $\mathbf{u} \in K^n$, $(ab)\mathbf{u}=a(b\mathbf{u})$.
   - This is true because scalar multiplication is associative.

10. Identity element of scalar multiplication: For any vector $\mathbf{u} \in K^n$, $1\mathbf{u}=\mathbf{u}$.
   - This is true because multiplication by the scalar 1 is the identity operation on $K$.

Therefore, $K^n$ satisfies all ten axioms of a vector space, and is thus a vector space over $K$ when $K$ is a field.
    
