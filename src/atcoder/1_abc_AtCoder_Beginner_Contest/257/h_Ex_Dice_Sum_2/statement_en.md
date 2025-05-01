
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
The six-sided dice speciality shop "Saikoroya" sells $N$dice.  The $i$-th die (singular of dice) has $A_{i,1},A_{i,2},\ldots,A_{i,6}$written on its each side, and has a price of $C_i$.
</p>

<p>
Takahashi is going to choose exactly $K$of them and buy them.
</p>

<p>
Currently, "Saikoroya" is conducting a promotion: Takahashi may roll each of the purchased dice once and claim money whose amount is equal to the square of the sum of the numbers shown by the dice.  Here, each die shows one of the six numbers uniformly at random and independently.
</p>

<p>
Maximize the expected value of (the amount of money he claims) - (the sum of money he pays for the purchased $K$dice) by properly choosing $K$dice to buy.  Print the maximized expected value modulo $998244353$.
</p>

<details>

<summary>
Definition of the expected value modulo $998244353$
</summary>

<p>
We can prove that the sought expected value is always a rational number.
Moreover, under the Constraints of this problem, the sought expected value can be expressed by an irreducible fraction $\frac{y}{x}$where $x$is indivisible by $998244353$.
</p>

<p>
In this case, we can uniquely determine the integer $z$between $0$and $998244352$(inclusive) such that $xz \equiv y \pmod{998244353}$.  Print such $z$.
</p>

</details>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 1000$
</li>

<li>
$1 \leq K \leq N$
</li>

<li>
$1 \leq C_i \leq 10^5$
</li>

<li>
$1 \leq A_{i,j} \leq 10^5$
</li>

<li>
All values in input are integers.
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
Input is given from Standard Input in the following format:
</p>

<div>

$N$$K$$C_1$$C_2$$\ldots$$C_N$$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,6}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,6}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
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
1 2 3
1 1 1 1 1 1
2 2 2 2 2 2
3 3 3 3 3 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

20

</div>

<p>
If he buys the $2$-nd and $3$-rd dice, the expected value of (the amount of money he claims) - (the sum of money he pays for the purchased $K$dice) equals $(2 + 3)^2 - (2 + 3) = 20$, which is the maximum expected value.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

10 5
2 5 6 5 2 1 7 9 7 2
5 5 2 4 7 6
2 2 8 7 7 9
8 1 9 6 10 8
8 6 10 3 3 9
1 10 5 8 1 10
7 8 4 8 6 5
1 10 2 5 1 7
7 4 1 4 5 4
5 10 1 5 1 2
5 1 2 3 6 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1014

</div>

</section>

</div>

</span>

</span>

</div>
