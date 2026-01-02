
<div>

<span>

<span>

<p>
Score : $1200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
For a length-$N$sequence of positive integers $A=(A_1,A_2,\dots,A_N)$, define $f(A)$as follows:
</p>

<ul>

<li>
The maximum value of $A_iA_j + A_k$over all triples of integers $(i,j,k)$satisfying $1 \le i < j < k \le N$.
</li>

</ul>

<p>
Find the number, modulo $998244353$, of length-$N$sequences $A$of positive integers with all elements between $1$and $M$, inclusive, such that $f(A) \le K$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \le N \le 10^9$
</li>

<li>
$1 \le M,K \le 10^4$
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

$N$$M$$K$
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

3 5 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

9

</div>

<p>
The sequences satisfying the condition are $(1,1,1),(1,1,2),(1,2,1),(2,1,1),(1,1,3),(1,2,2),(2,1,2),(1,3,1),(3,1,1)$, which is nine sequences.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 5 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

66

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

123 456 789

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

436486661

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

1000000000 10000 10000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

855626126

</div>

</section>

</div>

</span>

</span>

</div>
