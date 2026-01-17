
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a directed graph (not necessarily simple) with $N$vertices and $M$edges, where the vertices are numbered as vertices $1, 2, \ldots, N$.

The $i$-th $(1\leq i\leq M)$edge goes from vertex $U_i$to vertex $V_i$with cost $C_i$.
Additionally, the out-degree of each vertex is at most $4$.
</p>

<p>
Find all vertices $v$$(1\leq v\leq N)$that satisfy the following condition:
</p>

<blockquote>

<p>
There exists a path from vertex $1$to vertex $v$that satisfies both of the following conditions:
</p>

<ul>

<li>
It traverses exactly $L$edges. If the same edge is traversed multiple times, each traversal is counted.
</li>

<li>
The sum of the costs of the traversed edges is at least $S$and at most $T$. (If the same edge is traversed multiple times, the cost is added to the sum each time.)
</li>

</ul>

</blockquote>

<details>

<summary>
What is out-degree?
</summary>
The out-degree of vertex $u$refers to the number of edges going out from vertex $u$. Even if multiple edges go to the same vertex, they are counted separately.

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq M\leq 2\times 10^5$
</li>

<li>
$1\leq L \leq 10$
</li>

<li>
$1\leq S\leq T \leq 10^9$
</li>

<li>
$1\leq U_i,V_i\leq N$
</li>

<li>
$1\leq C_i\leq 10^8$
</li>

<li>
The out-degree of each vertex is at most $4$.
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

$N$$M$$L$$S$$T$$U_1$$V_1$$C_1$$U_2$$V_2$$C_2$$\vdots$$U_M$$V_M$$C_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the vertices that satisfy the condition in 
<strong>
ascending order
</strong>
, separated by spaces.

If there are no vertices that satisfy the condition, print an empty line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 8 3 80 100
1 2 20
1 3 70
2 1 30
2 5 10
3 2 10
3 4 30
3 5 20
5 1 70

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 5

</div>

<p>
The given graph is as shown in the left figure below. The cost of each edge is shown near the starting vertex of that edge.  
</p>

<p>

<img src="https://img.atcoder.jp/abc441/e8fc1c428ced9f3b279428f499247a8a.png">

</img>

</p>

<p>
Here, the following holds:
</p>

<ul>

<li>
For the path from vertex $1$to vertex $1$, consider vertex $1$$\to$vertex $2$$\to$vertex $5$$\to$vertex $1$(center of the figure above). This traverses exactly three edges, and the sum of the costs of the traversed edges is $20+10+70=100$, so it satisfies the condition.
</li>

<li>
There is no path from vertex $1$to vertex $2$that satisfies the condition. One path that traverses exactly three edges is vertex $1$$\to$vertex $2$$\to$vertex $1$$\to$vertex $2$, but the sum of the costs of the edges traversed in this path is $20+30+20=70$, which is less than $80$, so it does not satisfy the condition.
</li>

<li>
There is no path from vertex $1$to vertex $3$that satisfies the condition. One path that traverses exactly three edges is vertex $1$$\to$vertex $2$$\to$vertex $1$$\to$vertex $3$, but the sum of the costs of the edges traversed in this path is $20+30+70=120$, which is greater than $100$, so it does not satisfy the condition.
</li>

<li>
There is no path from vertex $1$to vertex $4$that satisfies the condition.
</li>

<li>
For the path from vertex $1$to vertex $5$, consider vertex $1$$\to$vertex $3$$\to$vertex $2$$\to$vertex $5$(right of the figure above). This traverses exactly three edges, and the sum of the costs of the traversed edges is $70+10+10=90$, so it satisfies the condition.
</li>

</ul>

<p>
Therefore, print $1$, $5$in this order. Note that you need to print those vertices that satisfy the condition in ascending order.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 1 1 1 100
2 3 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>


</div>

<p>
If there are no vertices that satisfy the condition, print an empty line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

2 5 3 1 100
1 1 1
2 2 100
1 2 1
1 2 1
1 2 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1 2

</div>

<p>
The graph may contain self-loops and multiple edges.

In this test case, the out-degrees from vertices $1$and $2$are $4$and $1$, respectively.
</p>

</section>

</div>

</span>

</span>

</div>
