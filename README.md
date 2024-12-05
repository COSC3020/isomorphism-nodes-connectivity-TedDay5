# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

A complete graph with n vertices needs to have every pair of vertices be connected by an edge.
$E = (n/2) = (n(n-1))/2$

$G_1$ and $G_2$ have the same amount of vertices since each vertex in $G_1$ paired with a vertex in $G_2$ since it's stated in the bijection ($f: V_1 \rightarrow V_2$).

The bijection exists since we can construct it.

(f: $V_1$ => $V_2$)

Graph $G_1$: { $V_1, E_1$ } has vertices $V_1$ = { $v_1, v_2, v_n$ }

Graph $G_2$: { $V_2, E_2$ } has vertices $V_2$ = { $w_1, w_2, w_n$ }

function f is a bijection since it's one-to-one and onto.
(f) means (f($v_i$) = $w_i$) for (i = 1, 2, n).
one-to-one by having each ($v_i$) map to a unique ($w_i$) meaning no two vertices in the ($V_1$) map is the same vertex in ($V_2$).
onto by each vertex ($w_i$) in ($V_2$) is the image of some vortex in ($v_i$) in ($V_1$), which means all vertices in ($V_2$) are included.
adjacency is preserved under (f) since $G_1$ and $G_2$ are complete graphs and every pair of vertices in ($V_1$) is connected by an edge and the same is true for ($V_2$).
Any pair (($v_i, v_j$) $\in E_1$):($v_i, v_j$) $\in E_1$ => (f($v_i$),f($v_j$)) = ($w_i, w_j$) $\in E_2$

A complete graph needs to have every vertex in $G_1$ be connected to every other vertex to show adjacency.
For all pairs of vertices $(u,v) \in V_1: (u,v) \in E_1 \rightarrow (f(u),f(v)) \in E_2$.
Since it's bijective every pair $(f(u),f(v)) \in E_2$ there is a cooresponding $(u,v) \in E_1$.
This means all adjacency relationships are preserved under f.

Since f has both adjacency and is a bijection.
$G_1$ and $G_2$ have both the same amount of vertices and edges.
$G_1$ and $G_2$ are isomorphic.

I used the lecture02-graphs slides for guidence and definitions.

“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”
