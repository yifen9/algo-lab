
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
For a sequence $A = (A_1, A_2, \ldots, A_{N+1})$of length $N+1$, consider obtaining a sequence $S = (S_1, S_2, \ldots, S_N)$of length $N$in the following way.
</p>

<ul>

<li>
For each $i$($1 \le i \le N$), let $S_i = A_i + A_{i+1}$.
</li>

</ul>

<p>
Find the number, modulo $10^9 + 7$, of sequences $S$of length $N$satisfying all of the following conditions.
</p>

<ul>

<li>
$S$is non-decreasing.
</li>

<li>
There exists a sequence $A$of length $N+1$consisting of integers between $0$and $M$, inclusive, such that $S$can be obtained from $A$in the way described above.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N, M \le 10^7$
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

$N$$M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer on a single line.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5

</div>

<p>
The possible sequences $A$are the following eight:
</p>

<ul>

<li>
$A = (0,0,0)$, for which $S = (0,0)$
</li>

<li>
$A = (0,0,1)$, for which $S = (0,1)$
</li>

<li>
$A = (0,1,0)$, for which $S = (1,1)$
</li>

<li>
$A = (0,1,1)$, for which $S = (1,2)$
</li>

<li>
$A = (1,0,0)$, for which $S = (1,0)$
</li>

<li>
$A = (1,0,1)$, for which $S = (1,1)$
</li>

<li>
$A = (1,1,0)$, for which $S = (2,1)$
</li>

<li>
$A = (1,1,1)$, for which $S = (2,2)$
</li>

</ul>

<p>
Among these, we have five distinct non-decreasing $S$: $(0,0),(0,1),(1,1),(1,2),(2,2)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

869121 10000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

767557322

</div>

</section>

</div>

</span>

</span>

</div>
