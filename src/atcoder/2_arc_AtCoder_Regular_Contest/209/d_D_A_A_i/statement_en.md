
<div>

<span>

<span>

<p>
Score : $900$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence $A = (A_1, A_2, \ldots, A_N)$of length $N$.
Each element is either an integer between $1$and $N$(inclusive) or $-1$.
</p>

<p>
Snuke has decided to create a new sequence using this sequence $A$.
</p>

<p>
First, replace all $-1$s in this sequence $A$with integers between $1$and $N$(inclusive).
</p>

<p>
Next, create a sequence $B = (B_1, B_2, \ldots, B_N)$of length $N$according to the following formula:
</p>

<ul>

<li>
$B_i=A_{A_i}$
</li>

</ul>

<p>
Find the lexicographically smallest possible sequence $B$.
</p>

<p>
You are given $T$test cases. Solve each of them.
</p>

<details>

<summary>
What is the lexicographical order of sequences?
</summary>

<p>
A sequence $C = (C_1,C_2,\ldots,C_N)$is 
<strong>
lexicographically smaller
</strong>
than a sequence $D = (D_1,D_2,\ldots,D_N)$if and only if there exists an integer $1 \leq i \leq N$such that both of the following hold:

</p>

<ul>

<li>
$(C_1,C_2,\ldots,C_{i-1}) = (D_1,D_2,\ldots,D_{i-1})$
</li>

<li>
$C_i$is (numerically) smaller than $D_i$.
</li>

</ul>

</details>

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
$1 \le N \le 5 \times 10^5$
</li>

<li>
$1 \le A_i \le N$or $A_i = -1$.
</li>

<li>
The sum of $N$over all test cases is at most $5\times 10^5$.
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

$N$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
For each test case, output the lexicographically smallest possible sequence $B$, separated by newlines.
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
4
4 -1 -1 3
5
5 4 5 3 1
7
-1 6 5 -1 7 -1 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3 1 4 1
1 3 1 5 5
1 1 7 1 6 1 1

</div>

<p>
In the first test case, the sequence $A$before Snuke's replacement is $(4,-1,-1,3)$.
</p>

<p>
Suppose he replaces it to get $A=(4, 3, 1, 3)$.
</p>

<p>
Then, $B=(A_4, A_3, A_1, A_3)=(3, 1, 4, 1)$.
</p>

<p>
It is impossible to obtain a lexicographically smaller sequence $B$than this.
</p>

</section>

</div>

</span>

</span>

</div>
