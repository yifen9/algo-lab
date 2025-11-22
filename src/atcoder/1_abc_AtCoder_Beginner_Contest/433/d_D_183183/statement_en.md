
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
For positive integers $x,y$, define $f(x,y)$as follows:
</p>

<ul>

<li>
The value obtained by interpreting $x,y$in decimal notation without leading zeros as strings, concatenating them in this order to obtain a string $S$, and then interpreting $S$as an integer in decimal notation.
</li>

</ul>

<p>
For example, $f(12,3) = 123$and $f(100,40)=10040$.
</p>

<p>
You are given positive integers $N,M$and a sequence of $N$positive integers $A=(A_1,A_2,\ldots,A_N)$.
</p>

<p>
Find the number of pairs of integers $(i,j)$that satisfy all of the following conditions.
</p>

<ul>

<li>
$1\le i,j\le N$
</li>

<li>
$f(A_i,A_j)$is a multiple of $M$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le N\le 2\times 10^5$
</li>

<li>
$1\le M\le 10^9$
</li>

<li>
$1\le A_i\le 10^9$
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

$N$$M$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the number of pairs of integers $(i,j)$that satisfy all the conditions.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 11
2 42

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<ul>

<li>
When $(i,j)=(1,1)$: $f(A_1,A_1)=22$is a multiple of $11$.
</li>

<li>
When $(i,j)=(1,2)$: $f(A_1,A_2)=242$is a multiple of $11$.
</li>

<li>
When $(i,j)=(2,1)$: $f(A_2,A_1)=422$is not a multiple of $11$.
</li>

<li>
When $(i,j)=(2,2)$: $f(A_2,A_2)=4242$is not a multiple of $11$.
</li>

</ul>

<p>
From the above, the pairs of integers that satisfy all the conditions are $(i,j)=(1,1),(1,2)$, which is two pairs. Thus, output $2$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 7
2 8 16 183

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

5 5
1000000000 1000000000 1000000000 1000000000 1000000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

25

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

12 13
80 68 862370 82217 8 56 5 168 672624 6 286057 11864

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

10

</div>

</section>

</div>

</span>

</span>

</div>
