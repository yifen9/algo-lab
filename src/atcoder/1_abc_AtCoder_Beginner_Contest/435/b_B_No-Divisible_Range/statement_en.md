
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
You are given a sequence of positive integers $A=(A_1,A_2,\ldots,A_N)$of length $N$.

Find the number of pairs of integers $(l,r)$satisfying $1\leq l\leq r\leq N$that satisfy the following condition:
</p>

<blockquote>

<p>
For every integer $i$satisfying $l\leq i\leq r$, $A_i$is 
<strong>
not
</strong>
a divisor of $A_l+A_{l+1}+\cdots+A_r$.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 50$
</li>

<li>
$1 \leq A_i \leq 1000$
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

$N$$A_1$$A_2$$\ldots$$A_N$
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

5
8 6 10 5 7

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
We have $A=(8,6,10,5,7)$.
</p>

<p>
For example, $(l,r)=(1,2)$satisfies the condition because $A_l+A_{l+1}+\cdots+A_r=A_1+A_2=14$, and neither $A_1=8$nor $A_2=6$is a divisor of $14$.

On the other hand, $(l,r)=(1,3)$does not satisfy the condition because $A_l+A_{l+1}+\cdots+A_r=A_1+A_2+A_3=24$, and $A_1=8$is a divisor of $24$.
</p>

<p>
The pairs that satisfy the condition are $(l,r)=(1,2), (1,4), (2,3), (2,4), (3,5), (4,5)$, which is six pairs, so output $6$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3
1 1 1

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

</span>

</span>

</div>
