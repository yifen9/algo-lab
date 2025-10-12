
<div>
﻿
<span>

<span>

<p>
Score : $350$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a simple undirected graph with $N$vertices and $M$edges.
The graph consists of vertex $1,$vertex $2,\ldots,$vertex $N$, and the $i$-th edge $(1\le i\le M)$connects vertices $u _ i$and $v _ i$.
</p>

<p>
You will perform the following operation zero or more times:
</p>

<ul>

<li>
Choose one edge that has not been deleted yet, and delete it.
</li>

</ul>

<p>
Your goal is to make the graph bipartite.
Find the minimum number of operations needed to make the graph after the operations bipartite.
</p>

<details>

<summary>
What it means for a graph to be simple?
</summary>

<p>
A graph is simple if and only if it has no self-loops (edges where $u _ i=v _ i$) or multi-edges (pairs of edges where $u _ i=u _ j$and $v _ i=v _ j$).
</p>

</details>

<details>

<summary>
What is a bipartite graph?
</summary>

<p>
A bipartite graph is a graph where it is possible to color each vertex black or white satisfying the following condition:
</p>

<ul>

<li>
For every edge, the two vertices connected by that edge have different colors.
</li>

</ul>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\le N\le10$
</li>

<li>
$1\le M\le\dfrac{N(N-1)}2$
</li>

<li>
$1\le u _ i\lt v _ i\le N\ (1\le i\le M)$
</li>

<li>
The given graph is simple.
</li>

<li>
All input values are integers.
</li>

</ul>

</section>

</div>

---

<div>

<div>

<section>

### **Input**

<p>
The input is given from Standard Input in the following format:
</p>

<div>

$N$$M$$u _ 1$$v _ 1$$u _ 2$$v _ 2$$\vdots$$u _ M$$v _ M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the number of operations that need to be performed to make the graph bipartite.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 8
1 2
1 3
1 4
2 3
2 5
3 4
3 5
4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
You can make the graph bipartite by deleting two edges: for example, the edge connecting vertices $1$and $3$, and the edge connecting vertices $3$and $5$.
</p>

<p>
It is impossible to make the graph bipartite by performing one or less operations, so print `2`.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 1
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
The graph is bipartite from the beginning.
Thus, the number of operations that need to be performed is $0$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 20
5 9
1 4
3 8
1 6
4 10
5 7
5 6
3 7
3 6
5 10
1 3
3 4
6 7
1 2
4 7
1 5
1 9
9 10
4 5
8 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
