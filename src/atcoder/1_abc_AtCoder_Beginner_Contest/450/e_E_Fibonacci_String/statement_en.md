
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
You are given strings $X$and $Y$. Define a sequence of strings $S_1, S_2, \dots$as follows.
</p>

<ul>

<li>
$S_1 = X$
</li>

<li>
$S_2 = Y$
</li>

<li>
For $i \geq 3$, $S_i$is the concatenation of $S_{i-1}$and $S_{i-2}$in this order.
</li>

</ul>

<p>
For each $i = 1, 2, \ldots, Q$, answer the following problem.
</p>

<p>
Problem: You are given integers $L_i, R_i$and a character $C_i$. Find how many times character $C_i$appears in the $L_i$-th through $R_i$-th characters of $S_{10^{18}}$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$X$and $Y$are strings of lowercase English letters of length between $1$and $10^4$, inclusive.
</li>

<li>
$1 \leq Q \leq 10^5$
</li>

<li>
$1 \leq L_i \leq R_i \leq 10^{18}$
</li>

<li>
$C_i$is a lowercase English letter.
</li>

<li>
All given numerical values are integers.
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

$X$$Y$$Q$$L_1$$R_1$$C_1$$L_2$$R_2$$C_2$$\vdots$$L_Q$$R_Q$$C_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.

The $i$-th line should contain how many times character $C_i$appears in the $L_i$-th through $R_i$-th characters of $S_{10^{18}}$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

a
b
6
2 7 a
1 3 b
3 7 b
1 9 c
1 1000000000000000000 b
1000000000000000000 1000000000000000000 a

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
2
3
0
618033988749894848
1

</div>

<p>
$S_3$, $S_4$, $S_5$are `ba`, `bab`, `babba`, respectively.
</p>

<p>
$S_{10^{18}}$is `babbababbabba...`, and the second through seventh characters contain three occurrences of `a`.
</p>

</section>

</div>

</span>

</span>

</div>
