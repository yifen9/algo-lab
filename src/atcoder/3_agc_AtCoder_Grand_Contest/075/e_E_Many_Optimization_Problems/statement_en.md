
<div>

<span>

<span>

<p>
Score : $1600$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<b>
Optimization Problem
</b>

<p>
You are given a length-$N$sequence of non-negative integers $A=(A_1,A_2,\dots,A_N)$. Also, there is a length-$N+1$sequence of non-negative integers $X=(0,0,\dots,0)$.
</p>

<p>
You will now perform the following operation for $i=1,2,\dots,N$:
</p>

<ul>

<li>
Choose an integer $v$satisfying $0 \le v \le A_i$, and add $v$and $A_i-v$to $X_i$and $X_{i+1}$, respectively.
</li>

</ul>

<p>
Find the minimum possible value of the maximum value of $X$at the end of the operations.

</p>

</blockquote>

<p>
You are given positive integers $N$, $M$, and a prime number $P$. Find the sum, modulo $P$, of the answers to the 
<b>
Optimization Problem
</b>
for all sequences $A=(A_1,A_2,\dots,A_N)$of non-negative integers with length $N$and sum $M$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 100$
</li>

<li>
$1 \le M \le 10^{18}$
</li>

<li>
$9 \times 10^8 \le P \le 10^9$
</li>

<li>
$P$is prime.
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

$N$$M$$P$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the sum, modulo $P$, of the answers to the 
<b>
Optimization Problem
</b>
.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 3 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

13

</div>

<p>
For example, we solve the 
<b>
Optimization Problem
</b>
for $A=(1,0,2)$. Here is a possible sequence of operations:
</p>

<ul>

<li>
For $i = 1$, let $v = 1$. $X$becomes $(1,0,0,0)$.
</li>

<li>
For $i = 2$, let $v = 0$. $X$remains $(1,0,0,0)$.
</li>

<li>
For $i = 3$, let $v = 1$. $X$becomes $(1,0,1,1)$.
</li>

</ul>

<p>
Since the maximum value of $X$cannot be made $0$or less, the answer is $1$.
</p>

<p>
There are six other sequences with answer $1$and three sequences with answer $2$, so the sum is $13$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 135 998244353

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

679877945

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

100 1000000000000000000 924844033

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

789282612

</div>

</section>

</div>

</span>

</span>

</div>
