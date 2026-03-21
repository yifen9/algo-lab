
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
There are $N$stations $1, 2, \dots, N$, arranged in a straight line from west to east in this order.

The AtCoder Railway train passes through these $N$stations and runs from west to east.

For any two integers $i, j$satisfying $1 \leq i \lt j \leq N$, the cost of boarding the train at station $i$and getting off at station $j$is $C_{i,j}$.
</p>

<p>
Determine whether there exist three integers $a, b, c$such that:
</p>

<ul>

<li>
$1 \leq a \lt b \lt c \leq N$
</li>

<li>
The total cost of boarding the train at station $a$, getting off at station $b$, then boarding the train again at station $b$, and getting off at station $c$is less than the cost of boarding the train at station $a$and getting off at station $c$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \leq N \leq 100$
</li>

<li>
$1 \leq C_{i,j} \leq 10^9$
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

$N$$C_{1,2}$$C_{1,3}$$\dots$$C_{1,N}$$C_{2,3}$$\dots$$C_{2,N}$$\vdots$$C_{N-1,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If there exist three integers $a, b, c$satisfying the conditions, output `Yes`; otherwise, output `No`, on a single line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
45 450
45

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes

</div>

<p>
Choosing $(a, b, c) = (1, 2, 3)$,

$C_{a,b}+C_{b,c}=C_{1,2}+C_{2,3}=45+45$

$C_{a,c}=C_{1,3}=450$

so the conditions are satisfied.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
25 40 65
30 55
25

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

No

</div>

<p>
No choice of $(a, b, c)$satisfies the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
