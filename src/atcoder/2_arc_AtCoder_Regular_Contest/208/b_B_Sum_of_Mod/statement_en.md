
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given positive integers $N$and $K$.
</p>

<p>
Find one length-$N$sequence of positive integers $A=(A_1,A_2,\ldots,A_N)$with the minimum value of $A_N$among the ones that satisfy all of the following conditions.
</p>

<ul>

<li>
$A$is non-decreasing. That is, $A_i \le A_{i+1}$for $1\le i\le N-1$.
</li>

<li>
$\displaystyle \sum_{i=1}^{N-1} (A_{i+1} \bmod A_i)=K$.
</li>

</ul>

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
$1\le T \le 10^5$
</li>

<li>
$2\le N \le 2\times 10^5$
</li>

<li>
The sum of $N$over all test cases is at most $2\times 10^5$.
</li>

<li>
$1\le K\le 10^9$
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

$N$$K$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for each test case in order, separated by newlines.
</p>

<p>
For each test case, print $A$that satisfies all conditions and has the minimum value of $A_N$in the following format:
</p>

<div>

$A_1$$A_2$$\ldots$$A_N$
</div>

<p>
If there are multiple $A$that satisfy all conditions and have the minimum value of $A_N$, any of them will be accepted.
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
5 3
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 2 3 4 5
4 7

</div>

<p>
Consider the first test case.
</p>

<p>
$A=(1,2,3,4,5)$is non-decreasing and satisfies $\displaystyle \sum_{i=1}^{N-1} (A_{i+1} \bmod A_i) = (2\bmod 1) + (3\bmod 2) + (4\bmod 3) + (5\bmod 4)=3=K$, so it satisfies all conditions.
</p>

<p>
There does not exist an $A$that satisfies all conditions and has a value of $A_N$less than $5$, so printing $A=(1,2,3,4,5)$will be accepted.
</p>

<p>
Other than this, printing $A=(2,3,4,5,5)$or $A=(2,3,3,5,5)$will also be accepted.
</p>

</section>

</div>

</span>

</span>

</div>
