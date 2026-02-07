
<div>

<span>

<span>

<p>
Score : $675$points
</p>

<div>

<section>

### **Problem Statement**

<p>
On a two-dimensional coordinate plane, there is a circle with center at point $(\frac{A}{C}, \frac{B}{C})$and radius $\frac{\sqrt{N}}{C}$.
Find the number, modulo $998244353$, of lattice points on the circumference of this circle.
</p>

<p>
$N$is given in its prime factorization form as $N=\prod_{i=1}^{M} P_i^{E_i}$.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$N \geq 1$
</li>

<li>
$2 \leq P_i \leq 100$
</li>

<li>
$P_i$are distinct primes.
</li>

<li>
$1 \leq E_i \leq 10^{18}$
</li>

<li>
$1 \leq C \leq 50$
</li>

<li>
$0 \leq A,B \lt C$
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

$A$$B$$C$$M$$P_1$$E_1$$P_2$$E_2$$\vdots$$P_M$$E_M$
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

1 1 2 2
2 1
5 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

12

</div>

<p>
As shown in the figure below, there are $12$lattice points on the circumference.
</p>

<p>

<img src="https://img.atcoder.jp/abc444/f34d3c88f51a7a212173794f9b2546da.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1 5 14 4
2 1
5 1
13 1
17 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4

</div>

<p>
As shown in the figure below, there are $4$lattice points on the circumference.
</p>

<p>

<img src="https://img.atcoder.jp/abc444/88d8c0112cd1be716f7355fbaddc93ad.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

1 1 6 3
2 1
5 2
13 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

6

</div>

<p>
As shown in the figure below, there are $6$lattice points on the circumference.
</p>

<p>

<img src="https://img.atcoder.jp/abc444/fd322921f436a778b10d591f0aebcbe2.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

0 0 1 10
97 1000000000000000000
89 1000000000000000000
73 1000000000000000000
61 1000000000000000000
59 1000000000000000000
47 1000000000000000000
31 1000000000000000000
23 1000000000000000000
11 1000000000000000000
5 1000000000000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

7885876

</div>

<p>
Find the number modulo $998244353$.
</p>

</section>

</div>

</span>

</span>

</div>
