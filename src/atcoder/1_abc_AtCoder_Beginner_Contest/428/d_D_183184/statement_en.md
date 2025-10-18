
<div>

<span>

<span>

<p>
Score : $400$points
</p>

<div>

<section>

### **Problem Statement**

<p>
For positive integers $x$and $y$, define $f(x,y)$as follows:
</p>

<ul>

<li>
Let $z$be the string obtained by interpreting $x,y$in decimal notation as strings and concatenating them in this order. Let $f(x,y)$be the value when $z$is interpreted as an integer in decimal notation.
</li>

</ul>

<p>
For example, $f(3,14)=314,\ f(100,3)=1003$.
</p>

<p>
You are given positive integers $C$and $D$. Find the number of integers $x$that satisfy the following conditions:
</p>

<ul>

<li>
$1 \leq x \leq D$
</li>

<li>
$f(C, C+x)$is a perfect square.
</li>

</ul>

<p>
You are given $T$test cases, find the answer for each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T \leq 3 \times 10^5$
</li>

<li>
$1 \leq C \leq 2 \times 10^8$
</li>

<li>
$1 \leq D \leq 5 \times 10^9$
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

$T$$\textrm{case}_1$$\textrm{case}_2$$\vdots$$\textrm{case}_T$
</div>

<p>
$\textrm{case}_i$represents the $i$-th test case. Each test case is given in the following format:
</p>

<div>

$C$$D$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line ($1 \leq i \leq T$) should contain the answer to the $i$-th test case.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
4 80
183 5000
18 10
824 5000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
2
0
1421

</div>

<p>
For the first test case, there are three values of $x$that satisfy the conditions: $x = 5, 37, 80$.
</p>

<ul>

<li>
When $x=5$, $f(C, C+5) = f(4,9) = 49 = 7^2$
</li>

<li>
When $x=37$, $f(C, C+37) = f(4,41) = 441 = 21^2$
</li>

<li>
When $x=80$, $f(C, C+80) = f(4,84) = 484 = 22^2$
</li>

</ul>

<p>
For the second test case, there are two values of $x$that satisfy the conditions: $x = 1, 3133$.
</p>

<ul>

<li>
When $x=1$, $f(C, C+1) = f(183,184) = 183184 = 428^2$
</li>

<li>
When $x=3133$, $f(C, C+3133) = f(183,3316) = 1833316 = 1354^2$
</li>

</ul>

<p>
For the third test case, there are zero values of $x$that satisfy the conditions.
</p>

<p>
For the fourth test case, there are $1421$values of $x$that satisfy the conditions.
</p>

</section>

</div>

</span>

</span>

</div>
