
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
You are given an integer sequence $Y=(Y_1,Y_2,\ldots,Y_N)$of length $N$where each element is between $1$and $N$inclusive.
</p>

<p>
Determine whether there exists an $N \times N$integer matrix $A=(A_{i,j})$$(1\le i , j \le N)$that satisfies all of the following conditions, and if it exists, find one such matrix.
</p>

<ul>

<li>
$1\le A_{i,j} \le N$$(1\le i \le N, 1\le j\le N)$
</li>

<li>
$A_{i,j}=A_{j,i}$$(1\le i\le N, 1\le j\le N)$
</li>

<li>
$A_{i,j_1}\neq A_{i,j_2}$$(1\le i\le N, 1\le j_1 < j_2 \le N)$
</li>

<li>
$A_{i,Y_i}=1$$(1\le i\le N)$
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
$1\le T\le 5000$
</li>

<li>
$1\le N \le 500$
</li>

<li>
The sum of $N^2$over all test cases is at most $500^2$.
</li>

<li>
$1\le Y_i\le N$
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

$N$$Y_1$$Y_2$$\ldots$$Y_N$
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
For each test case, if there does not exist an $A$that satisfies all conditions, print `No`.
</p>

<p>
Otherwise, print $A$that satisfies all conditions in the following format:
</p>

<div>

Yes
$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,N}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,N}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,N}$
</div>

<p>
If there are multiple $A$that satisfy all conditions, any of them will be accepted.
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
3
1 3 2
3
1 2 3
1
1
5
1 3 2 5 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
1 2 3
2 3 1
3 1 2
No
Yes
1
Yes
1 2 5 4 3
2 3 1 5 4
5 1 4 3 2
4 5 3 2 1
3 4 2 1 5

</div>

<p>
Consider the first test case.
</p>

<p>
It can be verified that the $A$in the sample output satisfies all conditions. Other than this, for example, the following $A$will also be accepted:
</p>

<div>

1 3 2
3 2 1
2 1 3

</div>

</section>

</div>

</span>

</span>

</div>
