
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
You are given a sequence $A$of $N$non-negative integers.

Repeat the following operation until $A$has exactly one element.
</p>

<ul>

<li>
Choose two distinct integers $i$and $j$satisfying $1 \leq i, j \leq |A|$uniformly at random.
</li>

<li>
Let $a$and $b$be $A_i$and $A_j$, respectively.
</li>

<li>
Remove the $i$-th and $j$-th elements from $A$.
</li>

<li>
Append $a - b$to the end of $A$.
</li>

</ul>

<p>
Let $x$be the only element of $A$at the end.
Find the expected value of $x^2$, modulo $998244353$.
</p>

<details>

<summary>
Definition of expected value modulo $998244353$
</summary>

<p>
It can be proved that the expected value to be found is always a rational number. It can also be proved that under the constraints of this problem, when expressed as an irreducible fraction $\frac{P}{Q}$, we have $Q \neq 0 \pmod{998244353}$. Thus, there is a unique integer $R$satisfying $R \times Q \equiv P \pmod{998244353}, 0 \leq R < 998244353$. Find this $R$.


</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq A_i \leq 998244352$
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

$N$$A_1$$A_2$$\dots$$A_N$
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

3
4 5 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

665496263

</div>

<p>
First, choosing $(i, j) = (3, 1)$makes the sequence $(5, -4)$.

Next, choosing $(i, j) = (1, 2)$makes the sequence $(9)$.

$x^2$equals $81$with probability $\frac{1}{3}$and $1$with probability $\frac{2}{3}$, so the expected value is $\frac{83}{3}$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
450 2026 3 21 100

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

669406799

</div>

</section>

</div>

</span>

</span>

</div>
