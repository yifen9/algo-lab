
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
You are given a positive integer $N$and a sequence of integers $A = (A_1, A_2, \ldots, A_N)$. Each $A_i$satisfies $-1 \leq A_i \leq N-1$, and for $1 \leq i < j \leq N$, if $A_i \neq -1$and $A_j \neq -1$, then $A_i \neq A_j$.
</p>

<p>
Answer the following query $Q$times.
</p>

<ul>

<li>
You are given integers $l, r\ (1 \leq l \leq r \leq N)$.

Find the sum, modulo $998244353$, of $\mathrm{mex}(\lbrace P_l, P_{l+1}, \ldots, P_r \rbrace)$over all permutations $P = (P_1, P_2, \ldots, P_N)$of $(0, 1, \ldots, N-1)$satisfying $A_i \neq -1 \implies P_i = A_i$.
</li>

</ul>

<details>

<summary>
What is $\mathrm{mex}(S)$?
</summary>
For a set $S$of non-negative integers, $\mathrm{mex}(S)$is defined as the smallest non-negative integer not contained in $S$.

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 5000$
</li>

<li>
$1 \leq Q \leq 5 \times 10^5$
</li>

<li>
$-1 \leq A_i \leq N-1$
</li>

<li>
For $1 \leq i < j \leq N$, if $A_i \neq -1$and $A_j \neq -1$, then $A_i \neq A_j$.
</li>

<li>
For each query, $1 \leq l \leq r \leq N$.
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

$N$$Q$$A_1$$A_2$$\ldots$$A_N$$\mathrm{query}_1$$\mathrm{query}_2$$\vdots$$\mathrm{query}_Q$
</div>

<p>
Each query is given in the following format:
</p>

<div>

$l$$r$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line should contain the answer to $\mathrm{query}_i$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 4
0 -1 -1
1 1
2 2
1 2
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
0
3
6

</div>

<p>
The permutations $P$satisfying $A_i \neq -1 \implies P_i = A_i$are $(0, 1, 2)$and $(0, 2, 1)$. Thus, the answer to each query is computed as follows.
</p>

<ul>

<li>
The answer to the first query is $\mathrm{mex}(\lbrace 0 \rbrace) + \mathrm{mex}(\lbrace 0 \rbrace) = 1 + 1 = 2$.
</li>

<li>
The answer to the second query is $\mathrm{mex}(\lbrace 1 \rbrace) + \mathrm{mex}(\lbrace 2 \rbrace) = 0 + 0 = 0$.
</li>

<li>
The answer to the third query is $\mathrm{mex}(\lbrace 0, 1 \rbrace) + \mathrm{mex}(\lbrace 0, 2 \rbrace) = 2 + 1 = 3$.
</li>

<li>
The answer to the fourth query is $\mathrm{mex}(\lbrace 0, 1, 2 \rbrace) + \mathrm{mex}(\lbrace 0, 2, 1 \rbrace) = 3 + 3 = 6$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5 3
-1 2 -1 -1 1
1 4
3 5
1 5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

6
8
30

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

15 1
-1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1
1 15

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

612227903

</div>

</section>

</div>

</span>

</span>

</div>
