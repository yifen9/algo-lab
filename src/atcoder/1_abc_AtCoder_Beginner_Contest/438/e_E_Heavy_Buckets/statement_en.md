
<div>

<span>

<span>

<p>
Score : $475$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N$people and $N$buckets. Both the people and buckets are numbered $1, 2, \ldots, N$.
</p>

<p>
Initially, person $i$holds only bucket $i$, and bucket $i$is empty.
</p>

<p>
From now on, the following operation will be performed $10^9$times:
</p>

<ul>

<li>
For $i = 1, 2, \ldots, N$
<strong>
simultaneously
</strong>
, person $i$adds $i$units of water to each of the buckets they are holding and passes those buckets to person $A_i$.
</li>

</ul>

<p>
Here, there is no limit on the amount of water that can be put in a bucket.
</p>

<p>
For $i = 1, 2, \ldots, Q$, answer the following queries:
</p>

<ul>

<li>
Find the amount of water in bucket $B_i$immediately after the $T_i$-th operation.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq Q \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i \leq N$
</li>

<li>
$1 \leq T_i \leq 10^9$
</li>

<li>
$1 \leq B_i \leq N$
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

$N$$Q$$A_1$$A_2$$\ldots$$A_N$$T_1$$B_1$$T_2$$B_2$$\vdots$$T_Q$$B_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines. The $i$-th line should contain the answer to the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 6
3 4 2 2 5
4 3
6 5
1 4
10 1
10 2
1000000000 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

11
30
4
28
30
2999999998

</div>

<p>
We will explain the first query.
</p>

<p>
Initially, bucket $3$is held by person $3$.
</p>

<p>
Immediately after the $1$-st operation, bucket $3$is held by person $2$and contains $3$units of water.
</p>

<p>
Immediately after the $2$-nd operation, bucket $3$is held by person $4$and contains $5$units of water.
</p>

<p>
Immediately after the $3$-rd operation, bucket $3$is held by person $2$and contains $9$units of water.
</p>

<p>
Immediately after the $4$-th operation, bucket $3$is held by person $4$and contains $11$units of water.
</p>

<p>
Thus, the answer to the first query is $11$.
</p>

</section>

</div>

</span>

</span>

</div>
