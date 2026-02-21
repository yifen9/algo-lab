
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a directed graph $G$with $N$vertices and $M$edges.

The vertices of $G$are numbered as vertex $1$, vertex $2$, $\ldots$, vertex $N$, and the $i$-th edge ($1\leq i\leq M$) goes from vertex $U_i$to vertex $V_i$.
</p>

<p>
Solve the following problem for $k=1,2,\ldots,N$.
</p>

<blockquote>

<p>
Takahashi's goal is to delete some (possibly zero) vertices from $G$, along with all edges having those vertices as an endpoint, so that the following condition is satisfied.
</p>

<ul>

<li>
The only vertices reachable from vertex $1$by traversing zero or more edges are vertices $1,2,\ldots,k$.
</li>

</ul>

<p>
Determine whether he can achieve his goal, and if so, find the minimum number of vertices he needs to delete to achieve it.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N\leq 3\times 10^5$
</li>

<li>
$1\leq M\leq 3\times 10^5$
</li>

<li>
$1\leq U_i,V_i\leq N$
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
Output $N$lines.

The $i$-th line ($1\leq i\leq N$) should contain the answer to the problem for $k=i$.

Here, for each problem, output $-1$if it is impossible for Takahashi to achieve his goal, and otherwise output the minimum number of vertices that need to be deleted to achieve his goal.
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
2 4
2 5
4 3
4 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
2
-1
1
0

</div>

<ul>

<li>
For $k=1$, the goal can be achieved by deleting vertex $2$. Note that vertices $3,4,5$are already unreachable from vertex $1$without deleting them. The goal cannot be achieved without deleting at least one vertex, so output $1$on the first line.
</li>

<li>
For $k=2$, the goal can be achieved by deleting vertices $4$and $5$. It is impossible to achieve the goal by deleting one or fewer vertices, so output $2$on the second line.
</li>

<li>
For $k=3$, Takahashi cannot achieve the goal no matter how he deletes vertices. Thus, output $-1$on the third line.
</li>

<li>
For $k=4$, the goal can be achieved by deleting vertex $5$. The goal cannot be achieved without deleting at least one vertex, so output $1$on the fourth line.
</li>

<li>
For $k=5$, the goal can be achieved without deleting any vertices. Thus, output $0$on the fifth line.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 5
1 1
1 2
3 1
3 1
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1
0
-1
-1
-1

</div>

<p>
$G$is not necessarily connected. Also, $G$may have multi-edges or self-loops.
</p>

</section>

</div>

</span>

</span>

</div>
