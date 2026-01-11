
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
There is a complete graph with four vertices numbered $1, 2, 3, 4$.
</p>

<p>
You will now assign weights to each of the six edges. Each weight should be a positive integer, and the sum of the six weights should be exactly $K$.

More formally, you choose positive integers $x_{i,j} \ (1\leq i<j\leq 4)$such that $\sum_{1\leq i<j\leq 4}x_{i,j}=K$, and assign weight $x_{i,j}$to the edge connecting $i$and $j$.
</p>

<p>
For this weighted graph $G$, let $f(G)$be the minimum sum of edge weights in a cycle that 
<strong>
passes through all vertices
</strong>
.
Find the sum, modulo $998244353$, of $f(G)$over all possible $G$.
</p>

<details>

<summary>
What is a complete graph?
</summary>

<p>
A complete graph is a graph with an edge between every pair of two distinct vertices.

</p>

</details>

<p>

</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$6 \le K \le 5000$
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

$K$
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

7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

24

</div>

<p>
The possible graphs are the ones where one of the six edges has weight $2$and the other edges have weight $1$.
There are six such graphs $G$, and we have $f(G)=4$for each of them, so the answer is $24$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2026

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

513760748

</div>

</section>

</div>

</span>

</span>

</div>
