
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
There is an undirected graph $G$with $N$vertices numbered $1$through $N$and zero edges.
</p>

<p>
$Q$queries are given. In the $i$-th query, an edge connecting vertices $u_i$and $v_i$is added to graph $G$.
</p>

<p>
Immediately after processing each query, determine whether it is possible to color each vertex of $G$white or black so that the following condition is satisfied, and if possible, find the minimum possible number of vertices colored black.
</p>

<ul>

<li>
For every edge, the two endpoints have different colors.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le Q \le 2 \times 10^5$
</li>

<li>
$1 \le u_i \lt v_i \le N$
</li>

<li>
$(u_i, v_i) \ne (u_j, v_j) \ (i \ne j)$
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

$N$$Q$$u_1$$v_1$$u_2$$v_2$$\vdots$$u_Q$$v_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
</p>

<p>
The $i$-th line should contain the following value for graph $G$immediately after processing the $i$-th query.
</p>

<ul>

<li>
If a valid coloring is possible, the minimum possible number of vertices colored black.
</li>

<li>
If no valid coloring is possible, $-1$.
</li>

</ul>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 4
1 2
2 3
3 4
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
1
2
-1

</div>

<p>
Immediately after processing queries $1, 2, 3$, a valid coloring exists.
</p>

<p>
For example, immediately after processing the third query, vertices $1, 2, 3, 4$can be colored `white`, `black`, `white`, `black`, respectively. No valid coloring with fewer `black`vertices exists, so output $2$.
</p>

<p>
Immediately after processing the fourth query, no valid coloring exists. Thus, output $-1$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 10
1 10
6 7
2 7
4 9
5 9
6 10
7 8
2 5
3 4
8 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1
2
2
3
3
3
3
4
4
4

</div>

</section>

</div>

</span>

</span>

</div>
