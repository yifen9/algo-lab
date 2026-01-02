
<div>

<span>

<span>

<p>
Score : $1400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Let $L=10^8$.
</p>

<p>
You are given an integer $N$and a non-negative integer sequence $A=(A_1,A_2,\cdots,A_M)$of length $M$($0 \leq A_i < L$).
For each $k=1,2,\cdots,N$, solve the following problem:
</p>

<p>
There are $k$red balls numbered from $1$to $k$and $k$blue balls numbered from $1$to $k$.
Now, you will write a real number on each ball in the following way.
Here, all random choices are independent.
</p>

<ul>

<li>

<p>
For each $1 \leq i \leq k$, the number written on red ball $i$is $L \times (i-1)+A_{j_i}$.
Here, $j_i$is an integer chosen uniformly at random from the range between $1$and $M$(inclusive).
</p>

</li>

<li>

<p>
For each $1 \leq i \leq k$, the number written on blue ball $i$is a 
<strong>
real number
</strong>
chosen uniformly at random from the range $[0,k \times L)$.
</p>

</li>

</ul>

<p>
Find the probability, modulo $998244353$, that the following condition is satisfied after writing numbers on all balls.
</p>

<ul>

<li>
For any real number $x$($0 \leq x \leq k \times L$), "the number of red balls with a number written that is at most $x$" $\geq$"the number of blue balls with a number written that is at most $x$".
</li>

</ul>

<details>

<summary>
Definition of probability modulo $998244353$
</summary>

<p>
It can be proved that the desired probability is always a rational number. Also, under the constraints of this problem, it can be proved that if the desired rational number is represented as an irreducible fraction $\frac{P}{Q}$, then $Q \neq 0 \pmod{998244353}$. Therefore, there uniquely exists an integer $R$satisfying $R \times Q \equiv P \pmod{998244353}, 0 \leq R \lt 998244353$. Output this $R$.


</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 250000$
</li>

<li>
$1 \leq M \leq 250000$
</li>

<li>
$0 \leq A_i < L=10^8$
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

$N$$M$$A_1$$A_2$$\cdots$$A_M$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines.
The $i$-th line should contain the answer for $k=i$.
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
50000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

499122177
686292993

</div>

<ul>

<li>
$k=1$: The probability of satisfying the condition is $1/2$.
</li>

<li>
$k=2$: The probability of satisfying the condition is $5/16$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 5
78682095 25048034 71067122 94666780 1927105

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

741897823
406774904
435399949

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

10 7
40490214 25131781 2271243 52064315 34467030 27419560 56103210

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

457696464
497746652
679391958
742383895
245278311
709723420
729551291
1911348
414224424
650563524

</div>

</section>

</div>

</span>

</span>

</div>
