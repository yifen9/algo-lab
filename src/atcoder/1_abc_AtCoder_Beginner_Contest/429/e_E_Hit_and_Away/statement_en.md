
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a simple connected undirected graph $G$with $N$vertices and $M$edges.

The vertices and edges of $G$are numbered as vertices $1,2,\ldots,N$and edges $1,2,\ldots,M$, respectively,
and edge $i$connects vertices $U_i$and $V_i$.

You can move bidirectionally between vertices connected by an edge in time $1$.
</p>

<p>
Additionally, each vertex is either safe or dangerous, and this state is given by a string $S$of length $N$consisting of `S`and `D`.

Specifically, vertex $i$is safe when the $i$-th character $(1\leq i\leq N)$of $S$is `S`, and vertex $i$is dangerous when it is `D`.

It is guaranteed that there are at least two safe vertices and at least one dangerous vertex.
</p>

<p>
For each dangerous vertex $v$, find the following value:
</p>

<blockquote>

<p>
The minimum possible time to start from some safe vertex, pass through $v$, and move to a safe vertex 
<strong>
different from the starting vertex
</strong>
.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3\leq N\leq 2\times 10^5$
</li>

<li>
$N-1\leq M\leq 2\times 10^5$
</li>

<li>
$1\leq U_i,V_i\leq N$
</li>

<li>
$U_i\neq V_i$
</li>

<li>
If $i\neq j$, then $\{ U_i,V_i \}\neq \{ U_j,V_j \}$.
</li>

<li>
$S$is a string of length $N$consisting of `S`and `D`.
</li>

<li>
$N,M,U_i,V_i$are all integers.
</li>

<li>
$G$is connected.
</li>

<li>
There are at least two safe vertices.
</li>

<li>
There is at least one dangerous vertex.
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

$N$$M$$U_1$$V_1$$U_2$$V_2$$\vdots$$U_M$$V_M$$S$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $K$be the number of dangerous vertices in $G$, and print $K$lines.

On the $i$-th line $(1\leq i\leq K)$, print the answer for the $i$-th dangerous vertex when the dangerous vertices are arranged in ascending order of vertex number.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 5
1 2
1 3
2 3
3 4
4 5
SSDDS

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
3

</div>

<p>
The dangerous vertices are (in ascending order of vertex number) vertices $3$and $4$.
</p>

<p>
For vertex $3$, moving from vertex $1$$\to$vertex $3$$\to$vertex $2$(for example) satisfies the condition.

The time required for this movement is $2$, and this is the minimum.

Therefore, print $2$on the $1$st line.
</p>

<p>
For vertex $4$, moving from vertex $1$$\to$vertex $3$$\to$vertex $4$$\to$vertex $5$(for example) satisfies the condition.

The time required for this movement is $3$, and there is no way to move that satisfies the condition with time $2$or less, so this is the minimum.

Therefore, print $3$on the $2$nd line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 2
1 2
2 3
SSD

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3

</div>

<p>
The dangerous vertex is vertex $3$.
</p>

<p>
Moving from vertex $1$$\to$vertex $2$$\to$vertex $3$$\to$vertex $2$(for example) satisfies the condition.

The time required for this movement is $3$, and this is the minimum.

Note that movements such as vertex $2$$\to$vertex $3$$\to$vertex $2$do not satisfy the condition that the destination is "different from the starting vertex".
</p>

</section>

</div>

</span>

</span>

</div>
