# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

# Solution

First, we need to establish what a completely connected graph is. Given two graphs $A = (V_A,E_A)$ and $B = (V_B,E_B)$ where $|V_A|=|V_B|=n$. If we assume A is completely connected, we are saying that for any two nodes ($u$ and $v$): 

$u,v \in V_A$, $(u,v) \in E_A$

The same is true for $B$: $x,y \in V_B$, $(x,y) \in E_B$

To prove isomorphism, we need to show there exists a bijective function $f: V_A \rightarrow V_B$ that preserves edges. Since $|V_A|=|V_B|=n$, we can create a one-to-one mapping between the vertices, call this mapping $f$. Here we can arbitrarily map each vertex in $V_A$ to a unique vertex in $V_B$ Now we need to show that this mapping preserves edges:

$(u,v) \in E_A \iff (f(u),f(v)) \in E_B$

This is always true because for any two vertices $u,v \in V_A$, $(u,v) \in E_A$ we get a complete graph. We also get a complete graph for $B$ for any two vertices $x,y \in V_B$, $(x,y) \in E_B$ Therefore, for any $u,v \in V_A$, both $(u,v) \in E_A$ and $(f(u),f(v)) \in E_B$ are always true

This means any bijective function $f$ from $V_A$ to $V_B$ will preserve the edge relationships making it an isomorphism.

# Disclaimer

I used [this](https://en.wikipedia.org/wiki/Graph_isomorphism) and [this](https://en.wikipedia.org/wiki/Isomorphism) to help with the understanding of the meaning behind the formal definition.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
