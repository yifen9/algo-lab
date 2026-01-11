
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N,M,X$.
</p>

<p>
Perform the following series of operations to create a sequence $A$of length $N$consisting of non-negative integers.
</p>

<ul>

<li>
Freely decide an integer sequence $A=(A_1,A_2)$of length $2$.
</li>

<li>
Then, perform the following operation $N-2$times on $A$.
</li>

<ul>

<li>
Let $k=|A|$. Let $x=A_{k-1}, y=A_k$. Append either $x+y$or $y-x$to the end of $A$.
</li>

</ul>

</ul>

<p>
A sequence $A$is a good sequence if and only if it satisfies the following:
</p>

<ul>

<li>
$0 \le A_i \le M \ (1 \le i \le N)$
</li>

<li>
$A_N=X$
</li>

</ul>

<p>
Find the sum, modulo $998244353$, of $A_1 \times A_2$over all good sequences that can be obtained by the operations.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq X \leq M \leq 2 \times 10^5$
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

$N$$M$$X$
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

3 4 3

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
Some possible sequences are $(0,3,3),(1,4,3),(2,1,3)$.
</p>

<p>
The sum of $A_1 \times A_2$over all possible sequences is $8$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

150000 160000 140000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

791841701

</div>

</section>

</div>

</span>

</span>

</div>
