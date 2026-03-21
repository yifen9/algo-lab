
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence $A$of $N$positive integers and a positive integer $K$.

You can perform the following operation on the sequence $A$any number of times.
</p>

<ul>

<li>
Choose an integer $i$with $1 \leq i \leq N$, and add $K$to $A_i$.
</li>

</ul>

<p>
Find the minimum possible value of $\max(A) - \min(A)$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq K \leq 10^9$
</li>

<li>
$1 \leq A_i \leq 10^9$
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

$N$$K$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer on a single line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 10
3 21 9

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
First, choosing $i=1$makes the sequence $A=(13,21,9)$.

Next, choosing $i=3$makes the sequence $A=(13,21,19)$.

Next, choosing $i=1$makes the sequence $A=(23,21,19)$.

At this point, $\max(A)-\min(A)=23-19=4$.

It is impossible to make $\max(A)-\min(A)$at most $3$, so the answer is $4$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 6
4 100 5 10 450

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

2

</div>

</section>

</div>

</span>

</span>

</div>
