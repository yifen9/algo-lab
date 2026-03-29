
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
You are given a positive integer $N$and a prime $P$.
</p>

<p>
There is a sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$where all elements are $0$.
</p>

<p>
You can repeat the following operation zero or more times.
</p>

<ul>

<li>
Choose a pair of integers $(l, r)\ (1\leq l\leq r\leq N)$. Replace each of $A_l,A_{l+1},\ldots,A_r$with $\dfrac{r(r-1)}{2}+l$.
</li>

</ul>

<p>
Find the number, modulo $P$, of sequences that can be obtained as $A$after performing operations.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 5000$
</li>

<li>
$P$is a prime satisfying $10^8\lt P\lt 10^9$.
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

$N$$P$
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

1 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
The two possible sequences $A$are $(0)$and $(1)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

2 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

7

</div>

<p>
The seven possible sequences $A$are $(0,0),(0,3),(1,0),(1,2),(1,3),(2,2),(2,3)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

38

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

4 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

282

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 5**

<div>

77 777777773

</div>

</section>

</div>

<div>

<section>

### **Sample Output 5**

<div>

112061248

</div>

</section>

</div>

</span>

</span>

</div>
