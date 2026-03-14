
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given positive integers $N, M$.
</p>

<p>
For a positive integer $d$, define the repunit with $d$digits as the integer $\displaystyle\sum_{i = 0}^{d - 1} 10^i$.
</p>

<p>
Find the number, modulo $998244353$, of integers that can be expressed as the sum of (not necessarily distinct) $N$repunits, each with at least $1$digit and at most $M$digits.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 10^5$
</li>

<li>
$1 \leq M \leq 10^9$
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

$N$$M$
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

2 3

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
We have $3$repunits with at least $1$digit and at most $3$digits: $1, 11, 111$. As the sum of $2$of them, we can express $6$integers: $2, 12, 22, 112, 122, 222$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

92378

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

12345 123456789

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

133394021

</div>

</section>

</div>

</span>

</span>

</div>
