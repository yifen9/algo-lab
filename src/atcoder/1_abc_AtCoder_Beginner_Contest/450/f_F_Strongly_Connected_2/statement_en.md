
<div>

<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a directed graph with $N$vertices and $N-1+M$edges, with edges and vertices numbered.

For $1 \leq i \leq M$, edge $i$is a directed edge from vertex $X_i$to vertex $Y_i$, and for $1 \leq i \leq N-1$, edge $M+i$is a directed edge from vertex $i+1$to vertex $i$.
</p>

<p>
There are $2^M$ways to choose some (possibly zero) edges from among edges $1, 2, \dots, M$. Among these ways, how many result in the graph being strongly connected after deleting the chosen edges? Find the count modulo $998244353$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq M \leq 2\times 10^5$
</li>

<li>
$1 \leq X_i < Y_i \leq N$
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

$N$$M$$X_1$$Y_1$$X_2$$Y_2$$\vdots$$X_M$$Y_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 3
1 4
1 3
2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5

</div>

<p>
The graph is strongly connected when the set of chosen edge indices is one of $\{\}, \{1\}, \{2\}, \{3\}, \{2,3\}$, giving five ways.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 11
1 4
1 4
3 9
2 5
3 4
9 10
6 9
4 10
1 3
8 10
4 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1297

</div>

<p>
The given graph may have multi-edges.
</p>

</section>

</div>

</span>

</span>

</div>
