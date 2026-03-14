
<div>

<span>

<span>

<p>
Score : $475$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N, M$and an integer sequence $A=(A_1,A_2,\ldots,A_N)$of length $N$where each element is between $1$and $M$, inclusive.
</p>

<p>
The following operation is performed $10^{100}$times on this integer sequence $A$:
</p>

<ul>

<li>
Let $v$be the integer between $1$and $M$, inclusive, with the fewest occurrences in $A$. If there are multiple such $v$, take the smallest among them. Then, append $v$to the end of $A$.
</li>

</ul>

<p>
You are given $Q$queries. The $i$-th query gives an integer $X_i$, so find the value of $A_{X_i}$after performing the operation $10^{100}$times.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N,M\le 5\times 10^5$
</li>

<li>
$1\le A_i \le M$
</li>

<li>
$1\le Q\le 2\times 10^5$
</li>

<li>
$1\le X_i \le 10^{18}$
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

$N$$M$$A_1$$A_2$$\ldots$$A_N$$Q$$X_1$$X_2$$\vdots$$X_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
</p>

<p>
The $i$-th line should contain the answer to the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 3
1 1 2
8
1
2
3
4
5
6
7
8

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
1
2
3
2
3
1
2

</div>

<p>
Initially, $A=(1,1,2)$. With each operation, $A$changes as follows:
</p>

<ul>

<li>
First operation: The counts of $1, 2, 3$in $A$are $2, 1, 0$respectively, so $v=3$. Append $v$to the end of $A$, giving $A=(1,1,2,3)$.
</li>

<li>
Second operation: The counts of $1, 2, 3$in $A$are $2, 1, 1$respectively, so $v=2$. Append $v$to the end of $A$, giving $A=(1,1,2,3,2)$.
</li>

<li>
Third operation: The counts of $1, 2, 3$in $A$are $2, 2, 1$respectively, so $v=3$. Append $v$to the end of $A$, giving $A=(1,1,2,3,2,3)$.
</li>

<li>
$\vdots$
</li>

</ul>

<p>
After performing the operation $10^{100}$times, $A$becomes $A=(1,1,2,3,2,3,1,2,\ldots)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7 30
20 26 3 14 4 4 9
10
31
9
21
23
97
99
30
79
57
3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

30
2
18
21
7
9
29
19
27
3

</div>

</section>

</div>

</span>

</span>

</div>
