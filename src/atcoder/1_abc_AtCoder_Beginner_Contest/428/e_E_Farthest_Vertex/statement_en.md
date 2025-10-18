
<div>

<span>

<span>

<p>
Score : $475$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a tree with $N$vertices numbered $1$to $N$. The $i$-th edge connects vertices $A_i$and $B_i$.

Define the distance between vertices $u$and $v$as the number of edges in the path with endpoints at vertices $u$and $v$. (This path is uniquely determined.)  
</p>

<p>
Solve the following problem for $v = 1, 2, \dots, N$.
</p>

<ul>

<li>
Among vertices $1, 2, \dots, N$, output the number of the vertex that has the maximum distance from vertex $v$. If there are multiple vertices that satisfy the condition, output 
<strong>
the vertex with the largest number
</strong>
.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 5 \times 10^5$
</li>

<li>
$1 \leq A_i \lt B_i \leq N$
</li>

<li>
The graph given in the input is a tree.
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

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_{N-1}$$B_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines. The $i$-th line should contain the answer for $v=i$.
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
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
3
1

</div>

<p>
The vertex with the maximum distance from vertex $1$is vertex $3$.

The vertices with the maximum distance from vertex $2$are vertices $1$and $3$. Among them, vertex $3$, which has the larger number, is the answer.

The vertex with the maximum distance from vertex $3$is vertex $1$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
1 2
2 3
2 4
1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4
5
5
5
4

</div>

</section>

</div>

</span>

</span>

</div>
