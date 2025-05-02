
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
There are $N$islands and $M$bidirectional bridges connecting two islands. The islands and bridges are numbered $1$, $2$, $\ldots$, $N$and $1$, $2$, $\ldots$, $M$, respectively.

Bridge $i$connects islands $U_i$and $V_i$, and the time it takes to cross it in either direction is $T_i$.

No bridge connects an island to itself, but it is possible for two islands to be directly connected by more than one bridge.

One can travel between any two islands using some bridges.
</p>

<p>
You are given $Q$queries, so answer each of them. The $i$-th query is as follows:
</p>

<blockquote>

<p>
You are given $K_i$distinct bridges: bridges $B_{i,1}, B_{i,2}, \ldots, B_{i,K_i}$.

Find the minimum time required to travel from island $1$to island $N$using each of these bridges at least once.

Only consider the time spent crossing bridges.

You can cross the given bridges in any order and in any direction.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 400$
</li>

<li>
$N-1 \leq M \leq 2 \times 10^5$
</li>

<li>
$1 \leq U_i < V_i \leq N$
</li>

<li>
$1 \leq T_i \leq 10^9$
</li>

<li>
$1 \leq Q \leq 3000$
</li>

<li>
$1 \leq K_i \leq 5$
</li>

<li>
$1 \leq B_{i,1} < B_{i,2} < \cdots < B_{i,K_i} \leq M$
</li>

<li>
All input values are integers.
</li>

<li>
It is possible to travel between any two islands using some bridges.
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

$N$$M$$U_1$$V_1$$T_1$$U_2$$V_2$$T_2$$\vdots$$U_M$$V_M$$T_M$$Q$$K_1$$B_{1,1}$$B_{1,2}$$\cdots$$B_{1,{K_1}}$$K_2$$B_{2,1}$$B_{2,2}$$\cdots$$B_{2,{K_2}}$$\vdots$$K_Q$$B_{Q,1}$$B_{Q,2}$$\cdots$$B_{Q,{K_Q}}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $Q$lines. The $i$-th line ($1 \leq i \leq Q$) should contain the answer to the $i$-th query as an integer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 5
1 2 10
1 3 20
1 3 30
2 3 15
2 3 25
2
1
1
2
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

25
70

</div>

<p>
For the first query, we need to find the minimum time to travel from island $1$to island $3$while using bridge $1$.
The minimum time is achieved by using bridge $1$to move from island $1$to island $2$, then using bridge $4$to move from island $2$to island $3$. The time taken is $10 + 15 = 25$.
Hence, print $25$on the first line.
</p>

<p>
For the second query, we need to find the minimum time to travel from island $1$to island $3$while using both bridges $3$and $5$.
The minimum time is achieved by using bridge $3$to move from island $1$to island $3$, then using bridge $5$to move to island $2$, and finally using bridge $4$to return to island $3$. The time taken is $30 + 25 + 15 = 70$.
Hence, print $70$on the second line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6 6
1 5 1
2 5 1
2 4 1
3 4 1
3 6 1
1 6 1
2
5
1 2 3 4 5
1
5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

5
3

</div>

<p>
For each query, you can cross the specified bridges in either direction.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 5
1 2 1000000000
2 3 1000000000
3 4 1000000000
4 5 1000000000
1 5 1000000000
1
1
3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

4000000000

</div>

<p>
Beware that the answer may not fit in a $32$-bit integer.
</p>

</section>

</div>

</span>

</span>

</div>
