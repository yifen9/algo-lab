
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
You are given a sequence $A=(A_1,A_2,\dots,A_N)$of length $N$.
</p>

<p>
Process $Q$queries in order.
Each query is in one of the following formats:
</p>

<ul>

<li>
`1 x`: Swap the values of $A_x$and $A_{x+1}$.
</li>

<li>
`2 l r`: Find the value of $\displaystyle \sum_{l\leq i\leq r} A_i$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N \leq 2\times 10^5$
</li>

<li>
$1\leq Q \leq 5\times 10^5$
</li>

<li>
$1\leq A_i \leq 10^4$
</li>

<li>
For queries of the first type, $1\leq x \leq N-1$.
</li>

<li>
For queries of the second type, $1\leq l\leq r \leq N$.
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

$N$$Q$$A_1$$A_2$$\dots$$A_N$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
Here, $\text{query}_i$represents the $i$-th query and is given in one of the following formats:
</p>

<div>

$1$$x$
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
Let $q$be the number of queries of the second type, and output $q$lines.
The $i$-th line $(1\leq i \leq q)$should contain the answer to the $i$-th query of the second type.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 4
2 7 1 8
1 2
2 1 2
1 1
2 2 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
17

</div>

<ul>

<li>
In the $1$-st query, swap the values of $A_2$and $A_3$. This makes $A=(2,1,7,8)$.
</li>

<li>
In the $2$-nd query, find the value of $A_1+A_2$. The answer is $2+1=3$.
</li>

<li>
In the $3$-rd query, swap the values of $A_1$and $A_2$. This makes $A=(1,2,7,8)$.
</li>

<li>
In the $4$-th query, find the value of $A_2+A_3+A_4$. The answer is $2+7+8=17$.
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
22 75 26 45 72 81 47 29
2 2 7
2 6 8
2 4 4
1 2
2 1 3
1 1
2 2 4
1 2
1 4
2 1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

346
157
45
123
142
26

</div>

</section>

</div>

</span>

</span>

</div>
