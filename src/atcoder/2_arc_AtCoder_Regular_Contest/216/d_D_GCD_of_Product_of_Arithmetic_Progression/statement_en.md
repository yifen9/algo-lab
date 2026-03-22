
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
You are given positive integers $N, B, C, D$.
</p>

<p>
For a non-negative integer $k$, define the integer $a_k$as the product of all terms of an arithmetic sequence with first term $Bk + C$, common difference $D$, and $N$terms; that is, $a_k = (Bk+C)(Bk+C+D)(Bk+C+2D)\dots(Bk+C+(N-1)D)$.
</p>

<p>
Find the greatest common divisor, modulo $998244353$, of $a_0, a_1, a_2, \ldots, a_N$.
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
$1 \leq T \leq 10^5$
</li>

<li>
$1 \leq N, B, C, D \leq 10^6$
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

$N$$B$$C$$D$
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

3
3 1 1 1
4 2 2 6
2026 3 22 216

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

6
128
114347907

</div>

<p>
For the first test case, $(a_0, a_1, a_2, a_3) = (1 \times 2 \times 3, 2 \times 3 \times 4, 3 \times 4 \times 5, 4 \times 5 \times 6) = (6, 24, 60, 120)$, and their greatest common divisor is $6$.
</p>

</section>

</div>

</span>

</span>

</div>
