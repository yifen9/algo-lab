
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence of length $N$, $A=(A_1,A_2,\ldots,A_N)$.

Find the number of triples of integers $(i,j,k)$satisfying $1\leq i<j<k\leq N$that satisfy the following condition:
</p>

<blockquote>

<p>
Exactly two distinct values are contained in $A_i,A_j,A_k$. That is, two of $A_i,A_j,A_k$are equal, and the remaining one is different.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3 \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq A_i \leq N$
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
Print the number of triples of integers that satisfy the condition.
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
3 2 5 2 2

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
For example, $(i,j,k)=(1,2,4)$satisfies the condition because exactly two distinct values, $2$and $3$, are contained in $A_1=3$, $A_2=2$, and $A_4=2$. 

Including this, the six triples $(i,j,k)=(1,2,4),(1,2,5),(1,4,5),(2,3,4),(2,3,5),(3,4,5)$satisfy the condition.

Therefore, print $6$.
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

<p>
There may be no triples that satisfy the condition.
</p>

</section>

</div>

</span>

</span>

</div>
