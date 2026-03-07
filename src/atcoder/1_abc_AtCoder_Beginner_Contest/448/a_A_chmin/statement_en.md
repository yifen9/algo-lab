
<div>

<span>

<span>

<p>
Score : $100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a length-$N$integer sequence $A=(A_1,A_2,\dots,A_N)$and an integer $X$.

For $i=1,2,\dots,N$in this order, do the following.
</p>

<ul>

<li>
If $A_i<X$, update $X=A_i$and output `1`.
</li>

<li>
Otherwise, output `0`.
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
$1 \le N,X,A_i \le 100$
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

$N$$X$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines.

The $k$-th line should contain the output for $i=k$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 10
6 4 7 1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
1
0
1
0

</div>

<ul>

<li>
Initially, $X=10$.
</li>

<li>
For $i=1$: since $A_1=6<X=10$, update $X=6$and output `1`.
</li>

<li>
For $i=2$: since $A_2=4<X=6$, update $X=4$and output `1`.
</li>

<li>
For $i=3$: since $A_3=7 \ge X=4$, output `0`.
</li>

<li>
For $i=4$: since $A_4=1<X=4$, update $X=1$and output `1`.
</li>

<li>
For $i=5$: since $A_5=3 \ge X=1$, output `0`.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 1
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

8 20
9 19 14 17 17 4 18 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1
0
0
0
0
1
0
0

</div>

</section>

</div>

</span>

</span>

</div>
