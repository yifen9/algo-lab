
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence of length $N$, $(A_1,\dots,A_N)$, and a positive integer $D$.
</p>

<p>
Find the number of pairs of integers $(L,R)$that satisfy both of the following conditions:
</p>

<ul>

<li>
$1 \leq L \leq R \leq N$
</li>

<li>
Any two elements of $(A_L,A_{L+1},\dots,A_R)$have a difference of at least $D$.
<ul>

<li>
That is, $|A_i-A_j|\geq D$for all pairs of integers $(i,j)$satisfying $L \leq i < j \leq R$.
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N \leq 4\times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
$1 \leq D \leq 10^9$
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

$N$$D$$A_1$$\dots$$A_N$
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

5 3
3 1 4 1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

8

</div>

<p>
The eight pairs $(1,1),(2,2),(3,3),(4,4),(5,5),(2,3),(3,4),(4,5)$satisfy the conditions.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

9 1
1 2 3 4 5 6 7 8 9

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

45

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6 1000000000
123456789 234567891 987654321 321987654 1000000000 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

6

</div>

</section>

</div>

</span>

</span>

</div>
