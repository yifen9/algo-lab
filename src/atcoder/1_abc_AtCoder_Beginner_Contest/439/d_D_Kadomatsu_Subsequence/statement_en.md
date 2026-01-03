
<div>

<span>

<span>

<p>
Score : $425$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $A=(A_1,A_2,\dots,A_N)$of length $N$.

Find the number of triples of integers $(i,j,k)$that satisfy all of the following:
</p>

<ul>

<li>
$1 \le i,j,k \le N$
</li>

<li>
$A_i : A_j : A_k = 7:5:3$
</li>

<li>
$\min(i,j,k) = j$or $\max(i,j,k) = j$.
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
$1 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le A_i \le 10^9$
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

$N$$A_1$$A_2$$\dots$$A_N$
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

10
3 10 7 10 7 6 7 6 5 14

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7

</div>

<p>
The seven triples of integers $(i,j,k)$that satisfy the conditions are:
</p>

<ul>

<li>
$(3,9,1)$
<ul>

<li>
$A_i : A_j : A_k = 7:5:3$, and $\max(i,j,k) = j$.
</li>

</ul>

</li>

<li>
$(5,9,1)$
<ul>

<li>
$A_i : A_j : A_k = 7:5:3$, and $\max(i,j,k) = j$.
</li>

</ul>

</li>

<li>
$(7,9,1)$
<ul>

<li>
$A_i : A_j : A_k = 7:5:3$, and $\max(i,j,k) = j$.
</li>

</ul>

</li>

<li>
$(10,2,6)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$, and $\min(i,j,k) = j$.
</li>

</ul>

</li>

<li>
$(10,2,8)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$, and $\min(i,j,k) = j$.
</li>

</ul>

</li>

<li>
$(10,4,6)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$, and $\min(i,j,k) = j$.
</li>

</ul>

</li>

<li>
$(10,4,8)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$, and $\min(i,j,k) = j$.
</li>

</ul>

</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6
210 210 210 210 210 210

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

21
49 30 50 21 35 15 21 70 35 9 50 70 21 49 30 50 70 15 9 21 30

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

34

</div>

</section>

</div>

</span>

</span>

</div>
