
<div>

<span>

<span>

<p>
Score : $650$points
</p>

<div>

<section>

### **Problem Statement**

<p>
For a string $A$consisting of `1`, `2`, $\dots$, `9`and `B`, define $f(A)$as the string obtained by the following procedure:
</p>

<ul>

<li>
Initially, there is an empty string $C$.
</li>

<li>
Perform the following operations in the order $i = 1, 2, \dots, |A|$:
<ul>

<li>
If $A_i$is one of `1`, `2`, $\dots$, `9`, append $A_i$to the end of $C$.
</li>

<li>
If $A_i =$`B`, delete the last character of $C$. However, if $C$is an empty string, do nothing.
</li>

</ul>

</li>

<li>
Let $f(A)$be $C$after completing all the above operations.
</li>

</ul>

<p>
You are given a string $S$of length $N$consisting of `1`, `2`, $\dots$, `9`, and `B`.

Process $Q$queries described below. Each query is of one of the following two types:
</p>

<ul>

<li>
$1\ \ x\ \ c$: Update $S_x$to $c$. (Here, $c$is `1`, `2`, $\dots$, `9`, or `B`.)
</li>

<li>
$2\ \ l\ \ r$: Let $T$be the string formed by extracting the $l$-th through $r$-th characters of $S$. Then, let $U=f(T)$. If $U$is an empty string, output $-1$; otherwise, output the remainder when the value of $U$regarded as a decimal integer is divided by $998244353$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 8 \times 10^6$
</li>

<li>
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$S$is a string of length $N$consisting of `1`, `2`, $\dots$, `9`, and `B`.
</li>

<li>
$1 \leq x \leq N$
</li>

<li>
$c$is `1`, `2`, $\dots$, `9`, or `B`.
</li>

<li>
$1 \leq l \leq r \leq N$
</li>

<li>
$N, Q, x, l, r$are integers.
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
The input is given from Standard Input in the following format, where $\mathrm{query}_i$denotes the $i$-th query.
</p>

<div>

$N$$Q$$S$$\mathrm{query}_1$$\mathrm{query}_2$$\vdots$$\mathrm{query}_Q$
</div>

<p>
Each query is given in one of the following two formats:
</p>

<div>

$1$$x$$c$
</div>

<div>

$2$$l$$r$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answers to the queries separated by newlines, following the instructions in the problem statement.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10 12
1234567891
2 5 7
2 2 8
2 1 10
1 3 B
1 4 B
2 2 4
2 2 8
2 1 10
1 7 B
2 3 9
1 3 4
2 1 10

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

567
2345678
236323538
-1
5678
567891
589
125891

</div>

<p>
For the first query, $T=U=$`567`. Thus, output $567$.

For the third query, $T=U=$`1234567891`. Thus, output $1234567891 \bmod 998244353 = 236323538$.

For the sixth query, $T=$`2BB`and $U$is an empty string. Thus, output $-1$.
</p>

</section>

</div>

</span>

</span>

</div>
