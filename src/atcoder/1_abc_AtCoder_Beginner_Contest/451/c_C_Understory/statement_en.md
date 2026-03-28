
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
Takahashi is managing the number of trees in his garden. Initially, there are no trees in the garden.
</p>

<p>
$Q$queries are given in order. Each query is one of the following two types. Immediately after processing each query, output the number of trees currently in the garden.
</p>

<ul>

<li>
`1 h`: Add one new tree of height $h$to the garden.
</li>

<li>
`2 h`: Remove all trees currently in the garden whose height is at most $h$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le Q \le 3 \times 10^5$
</li>

<li>
$1 \le h \le 10^9$
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

$Q$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
$\text{query}_i$, representing the $i$-th query, is one of the following two types:
</p>

<div>

$1$$h$
</div>

<div>

$2$$h$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.
</p>

<p>
The $i$-th line should contain the number of trees in the garden immediately after processing the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5
1 5
1 7
1 8
2 7
1 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1
2
3
1
2

</div>

<p>
The number of trees changes as follows.
</p>

<ul>

<li>
A tree of height $5$is added. The garden contains one tree of height $5$.
</li>

<li>
A tree of height $7$is added. The garden contains two trees of heights $5, 7$.
</li>

<li>
A tree of height $8$is added. The garden contains three trees of heights $5, 7, 8$.
</li>

<li>
Trees of height at most $7$are removed. The garden contains one tree of height $8$.
</li>

<li>
A tree of height $3$is added. The garden contains two trees of heights $8, 3$.
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

12
2 256601193
1 85138616
1 202564041
2 276477192
1 55551662
1 170271057
2 754166580
1 854388209
1 772036624
2 651124113
1 301137866
2 290875185

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0
1
2
0
1
2
0
1
2
2
3
3

</div>

</section>

</div>

</span>

</span>

</div>
