
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a simple connected undirected graph with $N$vertices and $M$edges. The $i$-th edge $(1\leq i\leq M)$is an undirected edge connecting vertices $U_i$and $V_i$.
</p>

<p>
Place signposts at all vertices as follows:
</p>

<ul>

<li>
At every vertex except vertex $1$, place a blue signpost pointing to one of its adjacent vertices.
</li>

<li>
At every vertex except vertex $2$, place a yellow signpost pointing to one of its adjacent vertices.
</li>

</ul>

<p>
Here, the two signposts at the same vertex must not point to the same vertex.
</p>

<p>
Determine whether it is possible to place signposts satisfying the following conditions, and if possible, output one way to place them:
</p>

<ul>

<li>
From any vertex other than vertex $1$, you can reach vertex $1$by repeatedly moving to the vertex pointed to by the blue signpost a finite number of times.
</li>

<li>
From any vertex other than vertex $2$, you can reach vertex $2$by repeatedly moving to the vertex pointed to by the yellow signpost a finite number of times.
</li>

</ul>

<p>
If there are multiple ways to place signposts satisfying the conditions, you may output any of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq M\leq 3\times 10^5$
</li>

<li>
$1\leq U_i\lt V_i\leq N$$(1\leq i\leq M)$
</li>

<li>
The given graph is simple and connected.
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

$N$$M$$U_1$$V_1$$U_2$$V_2$$\vdots$$U_M$$V_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If there is no way to place signposts satisfying the conditions, output `No`only.
</p>

<p>
If there is, output $N+1$lines.
</p>

<p>
The first line should contain `Yes`.
</p>

<p>
The second line should contain the number of the vertex pointed to by the yellow signpost at vertex $1$.
</p>

<p>
The third line should contain the number of the vertex pointed to by the blue signpost at vertex $2$.
</p>

<p>
The $i$-th line $(4\leq i\leq N+1)$should contain the number of the vertex pointed to by the blue signpost at vertex $i-1$and the number of the vertex pointed to by the yellow signpost at vertex $i-1$, in this order, separated by a space.
</p>

<p>
If there are multiple solutions, you may output any of them.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

7 8
1 3
3 4
4 5
1 5
4 6
2 6
2 7
4 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
5
6
4 1
5 6
1 4
4 2
4 2

</div>

<p>
Here, signposts are placed as shown in the figure below. For example, from vertex $3$:
</p>

<ul>

<li>
Following the blue signpost, you move as vertex $3\rightarrow 4\rightarrow 5\rightarrow 1$, eventually reaching vertex $1$.
</li>

<li>
Following the yellow signpost, you move as vertex $3\rightarrow 1\rightarrow 5\rightarrow 4 \rightarrow 6\rightarrow 2$, eventually reaching vertex $2$.
</li>

</ul>

<p>
You can also verify that following the blue signpost from vertex $2$leads to vertex $1$, and following the yellow signpost from vertex $1$leads to vertex $2$. The other vertices also satisfy the conditions.
</p>

<p>

<img src="https://img.atcoder.jp/arc211/b14d7aa0532d37600cd141d8f5f7f695.png">

</img>

</p>

<p>
There are multiple other solutions, but you must not have both the blue signpost and the yellow signpost at vertex $3$point to vertex $4$, because the signposts at the same vertex would point to the same vertex.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 12
1 3
3 4
4 5
1 5
4 6
2 6
2 7
4 7
4 8
8 9
9 10
8 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
There is no way to place signposts satisfying the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
