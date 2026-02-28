
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
You are given a simple connected undirected graph $G$with $N$vertices and $M$edges.
Here, $N \geq 2$.
The vertices are numbered $1$to $N$, and the edges are numbered $1$to $M$; edge $i$connects vertices $U_i$and $V_i$.
Each edge has a value called a 
<strong>
cost
</strong>
, and the cost of edge $i$is $2^i$.
</p>

<p>
You will now choose some edges of $G$to delete so that the number of connected components of $G$becomes exactly $2$.
(It can be proved that this is always achievable under the constraints of this problem.)
</p>

<p>
Find the minimum possible sum of costs of the deleted edges, modulo $998244353$.
(Note that you are not minimizing the remainder modulo $998244353$.)
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
$N-1 \leq M \leq \min\left(\frac{N(N-1)}{2}, 2\times 10^5\right)$
</li>

<li>
$1 \leq U_i < V_i \leq N$
</li>

<li>
$(U_i, V_i) \neq (U_j, V_j)$if $i \neq j$
</li>

<li>
$G$is connected.
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
Output the minimum possible sum of costs of the deleted edges, modulo $998244353$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 7
2 3
1 2
1 5
4 5
2 4
3 5
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

22

</div>

<p>

<img src="https://img.atcoder.jp/abc447/9a14605fcbaad3095d74d32d6cae6c55.png">

</img>

</p>

<p>
Deleting edges $1, 2, 4$(the edges shown as dashed lines in the figure above) makes the number of connected components of $G$exactly $2$.
</p>

<p>
In this case, the sum of costs of the deleted edges is $2^1+2^2+2^4=22$, which is the minimum.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 1
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

2

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8 16
2 7
5 7
6 8
1 7
4 7
1 3
2 8
5 8
4 8
2 5
3 4
3 8
1 4
1 8
4 6
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

54

</div>

</section>

</div>

</span>

</span>

</div>
