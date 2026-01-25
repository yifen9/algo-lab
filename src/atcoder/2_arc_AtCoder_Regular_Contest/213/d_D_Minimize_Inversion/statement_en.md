
<div>

<span>

<span>

<p>
Score : $1100$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given positive integers $N$and $K$satisfying $1\leq K\leq N$.
</p>

<p>
For a permutation $P = (P_{1}, P_{2}, \dots , P_{N})$of $(1, 2, \dots , N)$, define $f(P)$as follows:
</p>

<ul>

<li>
The minimum possible value of the number of inversions of a length-$N$integer sequence $A = (A_{1}, A_{2}, \dots, A_{N})$satisfying the following condition:
<ul>

<li>
$|A_{i}| = P_{i}$for every integer $1\leq i\leq N$.
</li>

</ul>

</li>

</ul>

<p>
For $a = 1, 2, \dots, N$, answer the following question:
</p>

<blockquote>

<p>
There are $(N - 1)!$permutations $P = (P_{1}, P_{2}, \dots , P_{N})$of $(1, 2, \dots , N)$satisfying $P_{K} = a$. Find the sum, modulo $998244353$, of $f(P)$over all of them.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq K\leq N\leq 2\times 10^{5}$
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

$N$$K$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines. The $i$-th line should contain the answer for $a = i$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
3
6
8

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

16 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

262718137
262718137
826158422
869037161
443336358
897729892
154945392
124681723
861272045
3176021
900143166
451899023
365015181
740245202
732524873
391198612

</div>

</section>

</div>

</span>

</span>

</div>
