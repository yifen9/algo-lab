
<div>

<span>

<span>

<p>
Score : $425$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a directed graph with $N$vertices and $M$edges.

The vertices are numbered from $1$to $N$, and the $i$-th edge is a directed edge from vertex $X_i$to vertex $Y_i$.

Initially, all vertices are white.
</p>

<p>
Process $Q$queries in order. Each query is of one of the following two types:
</p>

<ul>

<li>
`1 v`: Color vertex $v$black.
</li>

<li>
`2 v`: Determine whether it is possible to reach a black vertex by following edges from vertex $v$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 3\times 10^5$
</li>

<li>
$0\leq M \leq 3\times 10^5$
</li>

<li>
$1\leq Q \leq 3\times 10^5$
</li>

<li>
$1\leq X_i,Y_i \leq N$
</li>

<li>
There are no self-loops, that is, $X_i \neq Y_i$.
</li>

<li>
There are no multiple edges, that is, $(X_i,Y_i)$are distinct.
</li>

<li>
In queries, $1 \leq v \leq N$.
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

$N$$M$$X_1$$Y_1$$\vdots$$X_M$$Y_M$$Q$$\mathrm{query}_1$$\vdots$$\mathrm{query}_Q$
</div>

<p>
$\mathrm{query}_i$represents the $i$-th query and is given in one of the following formats:
</p>

<div>

$1$$v$
</div>

<div>

$2$$v$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $q$be the number of queries of the second type. Output $q$lines.
</p>

<p>
The $i$-th line should contain `Yes`if a black vertex is reachable in the $i$-th query of the second type, and `No`otherwise.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 6
1 2
2 3
3 1
4 5
1 4
2 5
5
1 3
2 1
2 4
1 5
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
No
Yes

</div>

<ul>

<li>
Initially, the given graph is as shown in the leftmost figure below.
</li>

<li>
By the first query, vertex $3$becomes black, as shown in the center figure.
</li>

<li>
In the second query, it is possible to reach black vertex $3$from vertex $1$.
</li>

<li>
In the third query, it is not possible to reach a black vertex from vertex $4$.
</li>

<li>
By the fourth query, vertex $5$becomes black, as shown in the rightmost figure.
</li>

<li>
In the fifth query, it is possible to reach black vertex $5$from vertex $4$.
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc435/82e480fb4420fdfd7a0f13168774c1fb.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
