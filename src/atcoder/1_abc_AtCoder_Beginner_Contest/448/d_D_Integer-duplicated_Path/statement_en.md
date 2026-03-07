
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
You are given a tree with $N$vertices numbered $1,2,\dots,N$. The $i$-th edge connects vertices $U_i$and $V_i$.

Each vertex $i$has an integer $A_i$written on it.
</p>

<p>
Answer the following problem for all $k=1,2,\dots,N$.
</p>

<ul>

<li>
Problem: Among the vertices on the simple path (a path that does not visit the same vertex more than once) from vertex $1$to vertex $k$, if there exist two distinct vertices with the same integer written on them, output `Yes`; otherwise, output `No`.
<ul>

<li>
It can be proved that the simple path connecting two vertices on a tree is unique.
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
All input values are integers.
</li>

<li>
$2 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i \le 10^9$
</li>

<li>
$1 \le U_i, V_i \le N$
</li>

<li>
The given graph is a tree.
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

$N$$A_1$$A_2$$\dots$$A_N$$U_1$$V_1$$U_2$$V_2$$\vdots$$U_{N-1}$$V_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines.

The $i$-th line should contain the answer to the problem for $k=i$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5
1 3 2 1 2
1 2
1 3
3 4
3 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

No
No
No
Yes
Yes

</div>

<ul>

<li>
For $k=1$: the path from vertex $1$to vertex $1$contains only vertex $1$. Since the path consists of only one vertex, the answer is `No`.
</li>

<li>
For $k=2$: the path from vertex $1$to vertex $2$contains vertices $1,2$, with integers $1,3$written on them respectively. Thus, the answer is `No`.
</li>

<li>
For $k=3$: the path from vertex $1$to vertex $3$contains vertices $1,3$, with integers $1,2$written on them respectively. Thus, the answer is `No`.
</li>

<li>
For $k=4$: the path from vertex $1$to vertex $4$contains vertices $1,3,4$, with integers $1,2,1$written on them respectively. Since vertices $1$and $4$on the path have the same integer $1$written on them, the answer is `Yes`.
</li>

<li>
For $k=5$: the path from vertex $1$to vertex $5$contains vertices $1,3,5$, with integers $1,2,2$written on them respectively. Since vertices $3$and $5$on the path have the same integer $2$written on them, the answer is `Yes`.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2
1000000000 1000000000
2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No
Yes

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
10 7 3 9 1 3 8 5 7 10
3 6
8 6
6 1
9 7
7 10
5 4
4 2
10 2
1 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

No
Yes
Yes
Yes
Yes
No
No
No
No
Yes

</div>

</section>

</div>

</span>

</span>

</div>
