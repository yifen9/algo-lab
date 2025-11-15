
<div>

<span>

<span>

<p>
Score : $575$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a sequence of positive integers $A=(A_1,A_2,\dots,A_N)$of length $N$and a sequence of positive integers $B=(B_1,B_2,\dots,B_M)$of length $M$.
</p>

<p>
Find the value of $\displaystyle \sum_{i=1}^{N} \sum_{j=1}^{M} \binom{A_i}{B_j}$, modulo $998244353$.
</p>

<p>
Here, $\displaystyle \binom{x}{y}$represents the number of ways to choose $y$objects from $x$objects (binomial coefficient), and particularly, it is $0$if $x < y$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N,M \leq 5\times 10^5$
</li>

<li>
$1\leq A_i,B_j \leq 5\times 10^5$
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

$N$$M$$A_1$$A_2$$\dots$$A_N$$B_1$$B_2$$\dots$$B_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 2
2 5 4
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

25

</div>

<p>
The answer is $\displaystyle \binom{2}{1}+\binom{2}{3}+\binom{5}{1}+\binom{5}{3}+\binom{4}{1}+\binom{4}{3}=2+0+5+10+4+4=25$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 4
2 5 1 5
2 1 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

65

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

6 8
203497 47202 407775 394325 463982 304784
468417 302156 131932 235902 395728 78537 223857 330739

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

602855848

</div>

</section>

</div>

</span>

</span>

</div>
