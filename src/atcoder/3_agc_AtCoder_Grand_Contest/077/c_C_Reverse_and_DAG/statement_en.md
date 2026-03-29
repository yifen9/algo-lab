
<div>

<span>

<span>

<p>
Score : $1000$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a simple directed graph $G$with $N$vertices and $M$edges. The vertices are numbered $1$through $N$, and the $i$-th edge goes from vertex $a_i$to vertex $b_i$. It is guaranteed that $(a_i,b_i)\neq (b_j,a_j)$for $i\neq j$. Also, an integer $K$with $2 \leq K \leq N-2$is given.
</p>

<p>
Determine whether it is possible to make $G$a graph with no directed cycles (DAG) by performing the following operation zero or more times.
</p>

<ul>

<li>
Choose a size-$K$subset $S$of $\lbrace 1,\ldots,N\rbrace$. For every directed edge whose both endpoints' numbers are in $S$, reverse its direction.
<ul>

<li>
That is, if there is an edge from vertex $u$to vertex $v\ (u,v\in S)$, delete that edge and add a directed edge from vertex $v$to vertex $u$. This operation is performed simultaneously for all applicable edges.
</li>

</ul>

</li>

</ul>

<p>
$T$test cases are given; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq  50000$
</li>

<li>
$4 \leq N \leq 2\times 10^5$
</li>

<li>
$0 \leq M \leq \min({N(N-1), 2\times 10^5})$
</li>

<li>
$2 \leq K \leq N-2$
</li>

<li>
$1 \leq a_i, b_i \leq N$
</li>

<li>
$a_i \neq b_i$
</li>

<li>
$(a_i, b_i) \neq (a_j, b_j)$and $(a_i,b_i) \neq (b_j,a_j)$for $i\neq j$.
</li>

<li>
The sum of $N$in each input is at most $2\times 10^5$.
</li>

<li>
The sum of $M$in each input is at most $2\times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$M$$K$$a_1$$b_1$$a_2$$b_2$$\vdots$$a_M$$b_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for $\mathrm{case}_1,\mathrm{case}_2,\ldots,\mathrm{case}_T$in this order in the following format.
</p>

<p>
Output `Yes`if it is possible to make $G$a graph with no directed cycles (DAG) by performing the operation zero or more times, and `No`otherwise.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
7 10 3
1 2
2 3
3 1
4 5
5 6
6 4
1 4
2 5
3 6
7 1
7 19 5
1 4
2 3
2 4
2 5
3 5
3 6
3 7
4 3
4 6
4 7
5 1
5 4
5 6
6 1
6 2
6 7
7 1
7 2
7 5
9 15 5
1 6
2 7
2 9
3 1
3 4
4 5
4 6
4 7
4 8
5 7
5 9
6 5
6 9
7 9
8 9

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

<p>
In the first test case, $G$can be made into a graph with no directed cycles by performing the following two operations.
</p>

<ul>

<li>

<p>
In the first operation, perform the operation with $S = \lbrace 1, 2,7 \rbrace$. The directed edges whose both endpoints' numbers are in $S$are the edge from vertex $1$to vertex $2$and the edge from vertex $7$to vertex $1$. The directions of these edges are reversed.
</p>

</li>

<li>

<p>
In the second operation, perform the operation with $S = \lbrace 4, 5,7 \rbrace$. The directed edge whose both endpoints' numbers are in $S$is the edge from vertex $4$to vertex $5$. The direction of this edge is reversed, and $G$becomes a graph with no directed cycles.
</p>

</li>

</ul>

<p>
In the second test case, it is impossible to make $G$a graph with no directed cycles regardless of the operations performed.
</p>

</section>

</div>

</span>

</span>

</div>
