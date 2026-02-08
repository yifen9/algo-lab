
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
You are given integer sequences of length $N$, $A = (A_1, \dots ,A_N)$and $B = (B_1, \dots ,B_N)$, and a positive integer $K$.
</p>

<p>
Each time you pay a cost of $1$, you can perform adjacent swaps 
<strong>
exactly $K$times
</strong>
. An adjacent swap refers to the following operation:
</p>

<ul>

<li>
Choose an integer $i$between $1$and $N-1$, inclusive, and swap $A_i$and $A_{i+1}$.
</li>

</ul>

<p>
Determine if it is possible to make $A$match $B$. If possible, find the minimum cost required to make them match.
</p>

<p>
You are given $T$test cases; find the answer for each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^5$
</li>

<li>
$2 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le K \le 10^9$
</li>

<li>
$1 \le A_i,B_i \le N$
</li>

<li>
$\{A_1,\dots ,A_N\}$and $\{B_1,\dots ,B_N\}$match as multisets.
</li>

<li>
The sum of $N$over all test cases is at most $3 \times 10^5$.
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

$N$$K$$A_1$$A_2$$\ldots$$A_N$$B_1$$B_2$$\ldots$$B_N$
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
The $i$-th line should contain the minimum cost if it is possible to make $A$match $B$for the $i$-th test case, and `-1`otherwise.
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
5 4
3 1 4 1 5
5 1 3 1 4
2 1000000000
1 2
2 1
10 13
1 2 3 4 5 6 7 8 9 10
10 9 8 7 6 5 4 3 2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
-1
5

</div>

<p>
For the first test case, it is possible to make $A$and $B$match with a cost of $2$by performing the following operations:
</p>

<ol>

<li>
Pay a cost of $1$, and choose $i$as $3,1,4,1$in order for each adjacent swap, making $A = (3,1,1,5,4)$.
</li>

<li>
Pay a cost of $1$, and choose $i$as $3,1,2,1$in order for each adjacent swap, making $A = (5,1,3,1,4)$.
</li>

</ol>

<p>
For the second test case, it is impossible to make $A$and $B$match regardless of the cost.
</p>

</section>

</div>

</span>

</span>

</div>
