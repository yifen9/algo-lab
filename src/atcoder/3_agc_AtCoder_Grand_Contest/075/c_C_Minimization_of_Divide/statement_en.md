
<div>

<span>

<span>

<p>
Score : $1200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given two length-$N$sequences of non-negative integers: $A=(A_1,A_2,\dots,A_N)$and $B=(B_1,B_2,\dots,B_N)$.
</p>

<p>
For a permutation $P=(P_1,P_2,\dots,P_N)$of $(1,2,\dots,N)$, define the cost of $P$as $\sum_{i=1}^{N} \left \lfloor \frac{A_{P_i}}{2^{B_i}} \right \rfloor$.
</p>

<p>
Find the number, modulo $998244353$, of permutations $P$that achieve the minimum cost.
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
$1 \le T \le 2 \times 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i \le 10^9$
</li>

<li>
$0 \le B_i \le 30$
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
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

$N$$A_1\ A_2\ \dots\ A_N$$B_1\ B_2\ \dots\ B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line $(1 \le i \le T)$should contain the answer for $\mathrm{case}_i$.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

7
2
5 9
0 1
3
3 4 10
0 1 2
4
1 2 3 4
0 0 1 1
5
1000000000 1000000000 1000000000 1000000000 1000000000
0 0 0 0 0
11
19 68 97 62 99 52 57 19 43 80 96
5 3 3 2 3 4 3 2 3 4 3
14
86 49 83 31 5 43 7 46 98 36 60 4 69 59
3 1 4 4 4 0 1 3 0 4 3 5 1 2
10
907139744 237517128 852012347 350549430 62876062 196019710 263351472 184393437 281593038 753973502
23 12 1 26 29 24 0 7 10 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
2
4
120
8640
15552
1

</div>

<p>
For the first test case, the cost for each $P$is as follows:
</p>

<ul>

<li>
For $P=(1,2)$, $\left \lfloor \frac{A_{1}}{2^{B_1}} \right \rfloor + \left \lfloor \frac{A_{2}}{2^{B_2}} \right \rfloor = \left \lfloor \frac{5}{1} \right \rfloor + \left \lfloor \frac{9}{2} \right \rfloor = 9$
</li>

<li>
For $P=(2,1)$, $\left \lfloor \frac{A_{2}}{2^{B_1}} \right \rfloor + \left \lfloor \frac{A_{1}}{2^{B_2}} \right \rfloor = \left \lfloor \frac{9}{1} \right \rfloor + \left \lfloor \frac{5}{2} \right \rfloor = 11$
</li>

</ul>

<p>
Thus, the minimum cost is $9$, and there is one permutation $P = (1,2)$that achieves it.
</p>

<p>
For the second test case, $P = (1,2,3),(2,1,3)$achieve the minimum cost of $7$.
</p>

<p>
For the third test case, $P = (1,2,3,4),(2,1,3,4),(1,2,4,3),(2,1,4,3)$achieve the minimum cost of $6$.
</p>

<p>
For the fourth test case, all permutations of $(1,2,3,4,5)$achieve the minimum cost of $5000000000$.
</p>

</section>

</div>

</span>

</span>

</div>
