# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Each pair of nodes in $G_1$ that have an edge between them should be able to be transformed by the bijection to an equivalent in $G_2$, ($u, v$) $\in E_1$ if $(f(u), f(v))$ $\in E_2$.
This means if the graphs don't have the same amount of nodes there could be a case where graph $G_1$ has an edge that's between two nodes but graph $G_2$ doesn't have one of these nodes, which leaves it without an equivalent edge.
This makes it so ($u, v$) $\in E_1$ if $(f(u), f(v))$ $\in E_2$ false.

Here's two example graphs that show how this problem can occur.

Graph $G_1$: {'1': {'2': A, '3': B}, '2': {'3': C}, '3': { }} has vertices {1, 2, 3} has edges $E_1$ = {(1, 2),(1, 3),(2, 3)}

Graph $G_2$: {'A': {'B': 1}, 'B': { }} has vertices {A, B} has edges $E_2$ = {(A, B)}

f(1) => A

f(2) => B

f(3) => doesn't have any equivalent

This means (1, 3) (2, 3) which are $\in E_1$ do not have the equivalent of $(f(1), f(3))$ and $(f(2), f(3))$ $\in E_2$
