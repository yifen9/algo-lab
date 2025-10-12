
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
For a positive integer $x$, define $f(x)$as the sum of the digits in the decimal representation of $x$. For example, $f(123) = 1 + 2 + 3 = 6$.
</p>

<p>
Define an infinite sequence $A = (A_0, A_1, A_2, \ldots)$by the following formula:
</p>

<ul>

<li>
$A_0 = 1$
</li>

<li>
For $i \geq 1$, $A_i = \displaystyle\sum_{j = 0}^{i - 1} f(A_j)$
</li>

</ul>

<p>
You are given a positive integer $N$. Find the value of $A_N$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$N$is an integer between $1$and $100$, inclusive.
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

$N$
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

6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

23

</div>

<ul>

<li>
$A_0 = 1$
</li>

<li>
$A_1 = f(A_0) = 1$
</li>

<li>
$A_2 = f(A_0) + f(A_1) = 2$
</li>

<li>
$A_3 = f(A_0) + f(A_1) + f(A_2) = 4$
</li>

<li>
$A_4 = f(A_0) + f(A_1) + f(A_2) + f(A_3) = 8$
</li>

<li>
$A_5 = f(A_0) + f(A_1) + f(A_2) + f(A_3) + f(A_4) = 16$
</li>

<li>
$A_6 = f(A_0) + f(A_1) + f(A_2) + f(A_3) + f(A_4) + f(A_5) = 23$
</li>

</ul>

<p>
Thus, $A_6 = 23$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

45

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

427

</div>

</section>

</div>

</span>

</span>

</div>
