
<div>

<span>

<span>

<p>
Score : $1000$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a permutation $P = (P_1, P_2, \ldots, P_N)$of $(1, 2, \ldots, N)$and a set of pairs of integers $S = \lbrace (x_1, y_1), (x_2, y_2), \ldots, (x_M, y_M) \rbrace$.
</p>

<p>
You can perform the following two types of operations any number of times in any order.
</p>

<ul>

<li>
Choose $(l, r)\ (1 \leq l < r \leq N)$such that $(P_l, P_r) \in S$or $(P_r, P_l) \in S$, and swap the $l$-th and $r$-th elements of $P$. That is, replace $P$with $(P_1, \ldots, P_{l-1}, P_r, P_{l+1}, \ldots, P_{r-1}, P_l, P_{r+1}, \ldots, P_N)$.
</li>

<li>
Choose $(l, r)\ (1 \leq l < r \leq N)$such that $(P_l, P_r) \in S$or $(P_r, P_l) \in S$, and reverse the elements from the $l$-th to the $r$-th of $P$. That is, replace $P$with $(P_1, \ldots, P_{l-1}, P_r, P_{r-1}, \ldots, P_{l+1}, P_l, P_{r+1}, \ldots, P_N)$.
</li>

</ul>

<p>
Find the lexicographically smallest permutation obtainable by the operations.
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
$1 \leq T \leq 3 \times 10^4$
</li>

<li>
$2 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq M \leq 2 \times 10^5$
</li>

<li>
$P$is a permutation of $(1, 2, \ldots, N)$.
</li>

<li>
$1 \leq x_i < y_i \leq N$
</li>

<li>
$(x_i, y_i) \neq (x_j, y_j)$if $i \neq j$.
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
</li>

<li>
The sum of $M$over all test cases is at most $2 \times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$M$$P_1$$P_2$$\ldots$$P_N$$x_1$$y_1$$x_2$$y_2$$\vdots$$x_M$$y_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line should contain the answer to $\mathrm{case}_i$.
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
6 2
1 3 2 5 4 6
1 4
2 5
8 5
7 3 2 8 6 5 1 4
1 8
2 5
3 4
7 8
5 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 2 5 3 4 6
1 2 3 7 5 6 8 4

</div>

<p>
For the first test case, you can obtain $P = (1, 2, 5, 3, 4, 6)$by performing the operations as follows.
</p>

<ul>

<li>
Initially, $P = (1, 3, 2, 5, 4, 6)$.
</li>

<li>
Reverse the elements from the first to the fifth with $(l, r) = (1, 5)\ ((P_l, P_r) = (1, 4) \in S)$. $P$becomes $(4, 5, 2, 3, 1, 6)$.
</li>

<li>
Swap the second and third elements with $(l, r) = (2, 3)\ ((P_r, P_l) = (2, 5) \in S)$. $P$becomes $(4, 2, 5, 3, 1, 6)$.
</li>

<li>
Swap the first and fifth elements with $(l, r) = (1, 5)\ ((P_r, P_l) = (1, 4) \in S)$. $P$becomes $(1, 2, 5, 3, 4, 6)$.
</li>

</ul>

<p>
This is the lexicographically smallest permutation obtainable by the operations.
</p>

</section>

</div>

</span>

</span>

</div>
