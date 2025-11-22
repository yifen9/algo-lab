
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given integers $N,M$, a sequence of $N$integers $X=(X_1,X_2,\ldots,X_N)$, and a sequence of $M$integers $Y=(Y_1,Y_2,\ldots,Y_M)$.
</p>

<p>
Determine whether there exists an $N$row by $M$column integer matrix $A=(A_{i,j})$$(1\le i\le N,\ 1\le j\le M)$that satisfies all of the following conditions, and if so, find one such matrix.
</p>

<ul>

<li>
$1\le A_{i,j} \le N\times M$
</li>

<li>
All $N\times M$elements of $A_{i,j}$are distinct.
</li>

<li>
$\displaystyle \max_{1\le j\le M} A_{i,j} = X_i$for $i=1,2,\ldots,N$.
</li>

<li>
$\displaystyle \max_{1\le i\le N} A_{i,j} = Y_j$for $j=1,2,\ldots,M$.
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
$1\le T\le 10^5$
</li>

<li>
$1\le N,M$
</li>

<li>
The sum of $N\times M$over all test cases is at most $2\times 10^5$.
</li>

<li>
$1\le X_i,Y_j\le N\times M$
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

$N$$M$$X_1$$X_2$$\ldots$$X_N$$Y_1$$Y_2$$\ldots$$Y_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for the test cases in order, separated by newlines.
</p>

<p>
For each test case, if there is no $A$that satisfies all the conditions, output `No`.
</p>

<p>
Otherwise, output $A$that satisfies all the conditions in the following format:
</p>

<div>

Yes
$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,M}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,M}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,M}$
</div>

<p>
If there are multiple $A$that satisfy the conditions, any of them will be accepted.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
2 3
5 6
5 3 6
3 3
5 4 6
6 2 4
5 4
18 20 19 14 17
18 20 14 15

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

Yes
5 1 4
2 3 6
No
Yes
18 12 4 9
13 20 1 10
16 19 6 8
2 5 14 3
11 17 7 15

</div>

<p>
Consider the first test case.
</p>

<p>
In the sample output, all elements of $A$are between $1$and $6$and are distinct, and furthermore,
</p>

<ul>

<li>
$\displaystyle \max_{1\le j\le 3} A_{1,j} =\max \lbrace 5,1,4\rbrace = 5 = X_1$
</li>

<li>
$\displaystyle\max_{1\le j\le 3} A_{2,j} =\max \lbrace 2,3,6\rbrace = 6 = X_2$
</li>

<li>
$\displaystyle\max_{1\le i\le 2} A_{i,1} =\max \lbrace 5,2\rbrace = 5 = Y_1$
</li>

<li>
$\displaystyle\max_{1\le i\le 2} A_{i,2} =\max \lbrace 1,3\rbrace = 3 = Y_2$
</li>

<li>
$\displaystyle\max_{1\le i\le 2} A_{i,3} =\max \lbrace 4,6\rbrace = 6 = Y_3$
</li>

</ul>

<p>
so all conditions are satisfied.
</p>

<p>
Other outputs, such as the following, are also accepted.
</p>

<div>

Yes
5 3 1
4 2 6

</div>

</section>

</div>

</span>

</span>

</div>
