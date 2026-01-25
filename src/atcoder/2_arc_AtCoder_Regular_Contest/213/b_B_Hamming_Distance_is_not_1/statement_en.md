
<div>

<span>

<span>

<p>
Score : $800$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given non-negative integers $q,L,R\;(q \in \{ 0,1\}, \; L \leq R)$.
Consider a set $S$that satisfies all of the following conditions.
</p>

<ul>

<li>
$S$consists of distinct integers between $L$and $R$, inclusive.
</li>

<li>
If $a \in S, \; b \in S, \; a \neq b$, then $a$and $b$differ in at least two digits in binary representation.
More formally, there exist at least two non-negative integers $i$such that $\left\lfloor\frac{a}{2^i}\right\rfloor$and $\left\lfloor\frac{b}{2^i}\right\rfloor$have different parities.
</li>

<li>
Among those satisfying the above two conditions, the number of elements is maximum.
</li>

</ul>

<p>
If $q=0$, find the number of elements in such a set $S$.

If $q=1$, construct one such set $S$.
</p>

<p>
For each input file, solve $T$test cases.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 2 \times 10^5$
</li>

<li>
$0 \leq q \leq 1$
</li>

<li>
$0 \leq L \leq  R \leq 10^{18}$
</li>

<li>
The sum of $q(R-L)$over all test cases is at most $5\times 10^6$.
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

$T$$case_1$$case_2$$\vdots$$case_T$
</div>

<p>
Each case is given in the following format:
</p>

<div>

$q$$L$$R$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers in a total of $T$lines.

The $t$-th line should contain the answer for the $t$-th test case.

For each test case, if $q=0$, print the number of elements in a set $S$that satisfies the conditions.

If $q=1$, for a set $S$that satisfies the conditions, let
</p>

<p>
$B_i=\begin{cases} 1 \; (S \text{ contains } i) \\ 0 \; (S \text{ does not contain } i) \end{cases}$
</p>

<p>
and output it in the following format:
</p>

<div>

$B_L$$B_{L+1}$$\dots$$B_R$
</div>

<p>
If there are multiple sets $S$that satisfy the conditions, you may print any of them.
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
1 0 3
0 1 2
1 213 213

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1001
2
1

</div>

<p>
In the first test case, $S=\{0,3\}$satisfies the conditions.
$S=\{1,2\}$also satisfies the conditions, so it is correct as well.

In the second test case, the only $S$that satisfies the conditions is $\{1,2\}$, whose number of elements is $2$.
</p>

</section>

</div>

</span>

</span>

</div>
