
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are two sequences $A=(A_1,\dots,A_N)$and $B=(B_1,\dots,B_N)$. You can perform the following three types of operations any number of times in any order:
</p>

<ul>

<li>
Choose an index $i$such that $A_i = -1$, and replace $A_i$with any non-negative integer.
</li>

<li>
Choose an index $i$such that $B_i = -1$, and replace $B_i$with any non-negative integer.
</li>

<li>
Rearrange the elements of sequence $A$in any order.
</li>

</ul>

<p>
Determine whether it is possible, after these operations, for all elements of $A$and $B$to be non-negative and satisfy $A_1 + B_1 = A_2 + B_2 = \dots = A_N + B_N$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 2000$
</li>

<li>
$-1 \leq A_i \leq 10^9$
</li>

<li>
$-1 \leq B_i \leq 10^9$
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

$N$$A_1$$A_2$$\ldots$$A_N$$B_1$$B_2$$\ldots$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible, after the operations, for all elements of $A$and $B$to be non-negative and satisfy $A_1 + B_1 = A_2 + B_2 = \dots = A_N + B_N$, print `Yes`. Otherwise, print `No`.
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
2 0 -1 3
3 -1 4 2

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
Consider the following operations:
</p>

<ul>

<li>
Replace $A_3$with $1$.
</li>

<li>
Replace $B_2$with $1$.
</li>

<li>
Rearrange $A$to $(1,3,0,2)$.
</li>

</ul>

<p>
After these operations, $A = (1,3,0,2)$and $B = (3,1,4,2)$: all elements of $A$and $B$are non-negative, and $A_1+B_1 = A_2+B_2 = A_3+B_3 = A_4+B_4 = 4$is satisfied.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
1 2 3
1 2 4

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
No matter how you perform the operations, it is impossible to satisfy $A_1+B_1 = A_2+B_2 = A_3+B_3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

3
1 2 -1
1 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

No

</div>

</section>

</div>

</span>

</span>

</div>
