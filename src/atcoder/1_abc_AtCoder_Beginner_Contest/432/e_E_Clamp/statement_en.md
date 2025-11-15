
<div>

<span>

<span>

<p>
Score : $450$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an integer sequence $A=(A_1, A_2, \dots, A_N)$of length $N$.
</p>

<p>
You are given $Q$queries, which you should process in order.
Each query is in one of the following formats:
</p>

<ul>

<li>
`1 x y`: Change the value of $A_x$to $y$.
</li>

<li>
`2 l r`: Find the value of $\displaystyle \sum_{1\leq i\leq N} \max(l, \min(r, A_i))$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N \leq 5\times 10^5$
</li>

<li>
$1\leq Q \leq 2\times 10^5$
</li>

<li>
$0\leq A_i \leq 5\times 10^5$
</li>

<li>
For queries of the first type,
<ul>

<li>
$1\leq x\leq N$
</li>

<li>
$0\leq y \leq 5\times 10^5$
</li>

</ul>

</li>

<li>
For queries of the second type,
<ul>

<li>
$0\leq l,r \leq 5\times 10^5$
</li>

</ul>

</li>

<li>
All inputs are integers.
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

$N$$Q$$A_1$$A_2$$\dots$$A_N$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
Here, $\text{query}_i\ (1\leq i\leq Q)$represents the $i$-th query and is given in one of the following formats:
</p>

<div>

$1$$x$$y$
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
Let $K$be the number of queries of the second type. Output $K$lines.
The $i$-th line ($1\leq i \leq K$) should contain the answer to the $i$-th query of the second type.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 4
4 3 2
1 1 7
2 3 5
1 2 0
2 4 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

11
12

</div>

<p>
Initially, $A=(4,3,2)$.
</p>

<ul>

<li>
First query: Change the value of $A_1$to $7$. $A$becomes $(7,3,2)$.
</li>

<li>
Second query: Output $\max(3, \min(5, 7))+\max(3, \min(5, 3))+\max(3, \min(5, 2))=5+3+3=11$.
</li>

<li>
Third query: Change the value of $A_2$to $0$. $A$becomes $(7,0,2)$.
</li>

<li>
Fourth query: Output $\max(4, \min(2, 7))+\max(4, \min(2, 0))+\max(4, \min(2, 2))=4+4+4=12$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

8 10
320 578 244 604 145 839 156 857
2 400 556
1 5 168
2 254 62
2 145 301
1 1 23
1 3 0
2 413 758
2 297 613
1 8 451
2 598 692

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

3824
2032
2073
4350
3596
4884

</div>

</section>

</div>

</span>

</span>

</div>
