
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
You are given strings $A$and $B$of length $N$consisting of `0`and `1`. Let $A_i$denote the $i$-th character of $A$.
</p>

<p>
You can perform the following operation any number of times, possibly zero.
</p>

<ul>

<li>
Choose an integer $i\ (2 \leq i \leq N-1)$satisfying $A_{i-1} = A_{i+1}$, and flip $A_i$(change `1`to `0`or `0`to `1`).
</li>

</ul>

<p>
Determine whether you can make $A$equal to $B$by repeating the operation, and if so, find the minimum number of operations required.
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
$1 \leq T \leq 2 \times 10^5$
</li>

<li>
$3 \leq N \leq 10^6$
</li>

<li>
$A$and $B$are strings of length $N$consisting of `0`and `1`.
</li>

<li>
$T$and $N$are integers.
</li>

<li>
The sum of $N$over all test cases is at most $10^6$.
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

$N$$A$$B$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers for $\mathrm{case}_1, \mathrm{case}_2, \ldots, \mathrm{case}_T$in the following format.
</p>

<p>
If it is impossible to make $A$equal to $B$, print `-1`.
</p>

<p>
If it is possible, print the minimum number of operations required.
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
4
0001
0111
6
101101
011100
5
10101
10101
10
0101000101
0011100111

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
-1
0
6

</div>

<p>
For the first test case, you can make $A$equal to $B$in two operations as follows.
</p>

<ol>

<li>
Choose $i = 2$. $A$becomes `0101`.
</li>

<li>
Choose $i = 3$. $A$becomes `0111`.
</li>

</ol>

<p>
For the second test case, it is impossible to make $A$equal to $B$no matter how you operate.
</p>

</section>

</div>

</span>

</span>

</div>
