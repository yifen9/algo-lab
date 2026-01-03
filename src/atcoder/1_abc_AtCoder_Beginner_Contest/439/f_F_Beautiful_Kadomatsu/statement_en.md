
<div>

<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
A sequence $a=(a_1,a_2,\dots,a_k)$of length $k$is defined to be 
<strong>
kadomatsu-like
</strong>
as follows:
</p>

<ul>

<li>
Let $x$be the number of integers $i$that satisfy $2 \le i \le k-1$, $a_{i-1} < a_i$, and $a_i > a_{i+1}$.
</li>

<li>
Let $y$be the number of integers $i$that satisfy $2 \le i \le k-1$, $a_{i-1} > a_i$, and $a_i < a_{i+1}$.
</li>

<li>
The sequence $a$is called 
<strong>
kadomatsu-like
</strong>
if and only if $x > y$.
</li>

</ul>

<p>
You are given a permutation $P$of $(1,2,\dots,N)$.

Find the number, modulo $998244353$, of (not necessarily contiguous) subsequences of $P$that are kadomatsu-like.
</p>

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
$P$is a permutation of $(1,2,\dots,N)$.
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

$N$$P_1$$P_2$$\dots$$P_N$
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

4
1 3 4 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4

</div>

<p>
Among the subsequences of $P$, the following four are kadomatsu-like:
</p>

<ul>

<li>
$(1,3,4,2)$
</li>

<li>
$(1,3,2)$
</li>

<li>
$(1,4,2)$
</li>

<li>
$(3,4,2)$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1
1

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

20
11 10 18 13 12 16 5 19 7 6 17 4 9 1 14 2 20 15 8 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

431610

</div>

<p>
For example, the subsequence $a=(10,13,12,5,7,9,20,3)$is kadomatsu-like.
</p>

<ul>

<li>
We have $a_{i-1} < a_i$and $a_i > a_{i+1}$for $i=2,7$, so $x=2$.
</li>

<li>
We have $a_{i-1} > a_i$and $a_i < a_{i+1}$for $i=4$, so $y=1$.
</li>

<li>
Since $x > y$, the subsequence $a$is kadomatsu-like.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
