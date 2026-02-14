
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given $N$strings $S_1,S_2,\dots,S_N$of odd lengths consisting of lowercase English letters.
</p>

<p>
Let $m$be the length of the longest string among $S_1,S_2,\dots,S_N$.
Find strings $T_1,T_2,\dots,T_N$satisfying the following condition.
</p>

<ul>

<li>
Condition: $T_i$is a string of length $m$formed by concatenating $k$copies of `.`, $S_i$, and $k$copies of `.`in this order, for some non-negative integer $k$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$N$is an integer between $1$and $100$, inclusive.
</li>

<li>
$S_i$is a string of odd length between $1$and $99$, inclusive, consisting of lowercase English letters.
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

$N$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines. The $i$-th line $(1 \leq i \leq N)$should contain $T_i$.
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
apple
blueberry
coconut
dragonfruit

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

...apple...
.blueberry.
..coconut..
dragonfruit

</div>

<p>
$m=11$, and $T_1,T_2,T_3,T_4$satisfy the condition in the problem statement for $k=3,1,2,0$, respectively.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6
abc
d
efghi
jkl
mnopq
r

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

.abc.
..d..
efghi
.jkl.
mnopq
..r..

</div>

</section>

</div>

</span>

</span>

</div>
