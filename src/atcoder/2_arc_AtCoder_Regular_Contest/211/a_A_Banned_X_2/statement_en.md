
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
You are given a length-$9$sequence of non-negative integers $A=(A_1,A_2,\dots,A_9)$. It is guaranteed that $2\leq \sum_{i=1}^{9}A_i$.
</p>

<p>
You can perform the following operation any number of times (possibly zero): choose one element of $A$and add $1$to it.
</p>

<p>
What is the minimum number of operations required so that there exists a sequence of positive integers $S$satisfying all of the following conditions?
</p>

<ul>

<li>
All elements of $S$are between $1$and $9$, inclusive.
</li>

<li>
$S$contains exactly $A_i$occurrences of $i$for each integer $i$such that $1\leq i\leq 9$. (Thus, the length of $S$is $\sum_{i=1}^{9}A_i$.)
</li>

<li>
No two adjacent elements sum to $10$.
</li>

</ul>

<p>
It can be proved that the goal can be achieved in a finite number of operations.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T\leq 10^3$
</li>

<li>
$0\leq A_i\leq 10^9$$(1\leq i\leq 9)$
</li>

<li>
$2\leq \sum_{i=1}^{9}A_i$
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$A_1$$A_2$$\dots$$A_9$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
</p>

<p>
The $i$-th line should contain the answer for the $i$-th test case.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2
0 0 0 1 0 1 0 0 0
2 1 1 0 0 0 0 0 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
0

</div>

<p>
For the first test case, initially, the possible values of $S$satisfying all conditions except the last one are $(4,6)$and $(6,4)$, neither of which satisfies the last condition. By choosing $A_8$and adding $1$to it, $S=(6,8,4)$satisfies all conditions.
</p>

<p>
For the second test case, $S=(1,2,3,1)$satisfies the conditions without any operations.
</p>

</section>

</div>

</span>

</span>

</div>
