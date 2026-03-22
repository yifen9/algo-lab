
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence of non-negative integers $A = (A_1, A_2, \ldots, A_N)$of length $N$.
</p>

<p>
Find the number of pairs of integers $(l, r)\ (1 \leq l \leq r \leq N)$such that $2^{A_l} + 2^{A_{l+1}} + \dots + 2^{A_r}$is a power of $2$. Here, a power of $2$is a number expressible as $2^k$for some non-negative integer $k$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq A_i \leq 2 \times 10^5$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
0 1 0 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

6

</div>

<p>
The pairs $(l, r)$satisfying the condition are $(1,1), (1,3), (1,4), (2,2), (3,3), (4,4)$, totaling six pairs.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
100 100 100 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

8

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10
3 2 2 3 2 4 1 1 0 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

19

</div>

</section>

</div>

</span>

</span>

</div>
