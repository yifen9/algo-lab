
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
AtCoder Restaurant was open for $N$days after opening.
</p>

<p>
On day $i$($1\leq i\leq N$) after opening, the following actions were performed.
</p>

<ul>

<li>
In the morning of day $i$, $A_i$eggs are purchased.
</li>

<li>
At noon on day $i$, $B_i$eggs are used. Here, 
<strong>
eggs in stock are used in the order they were purchased
</strong>
.
</li>

<li>
In the evening of day $i$, all eggs that have been stocked for $D$or more days are discarded.
</li>

</ul>

<p>
There were no eggs in stock before the morning of day $1$, and eggs never ran out at noon on any day.
</p>

<p>
Find how many eggs remain in the restaurant after the evening action on day $N$.
</p>

<p>
$T$test cases are given; solve each.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq T\leq 2\times 10^5$
</li>

<li>
$1 \leq D \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq A_i,B_i \leq 10$
</li>

<li>
Eggs never run out at noon on any of the $N$days.
</li>

<li>
For each input, the sum of $N$over all test cases is at most $2\times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
$\mathrm{case}_i$represents the $i$-th test case.

Each test case is given in the following format:
</p>

<div>

$N$$D$$A_1$$A_2$$\ldots$$A_N$$B_1$$B_2$$\ldots$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.

The $i$-th line ($1\leq i\leq T$) should contain the answer for the $i$-th test case.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3
3 1
7 2 3
1 3 2
3 2
7 2 3
1 3 2
2 1
2 1
1 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
5
0

</div>

<p>
In the first test case, the following actions are performed.
</p>

<ul>

<li>
Initially, AtCoder Restaurant has no eggs.
</li>

<li>
In the morning of day $1$, $7$eggs are purchased. The restaurant has $7$eggs stocked on day $1$.
</li>

<li>
At noon on day $1$, $1$egg is used. The restaurant has $6$eggs stocked on day $1$remaining.
</li>

<li>
In the evening of day $1$, no eggs are discarded. The restaurant has $6$eggs stocked on day $1$remaining.
</li>

<li>
In the morning of day $2$, $2$eggs are purchased. The restaurant has $6$eggs stocked on day $1$and $2$eggs stocked on day $2$.
</li>

<li>
At noon on day $2$, $3$eggs are used. The restaurant has $3$eggs stocked on day $1$and $2$eggs stocked on day $2$remaining.
</li>

<li>
In the evening of day $2$, the eggs stocked on day $1$are discarded. The restaurant has $2$eggs stocked on day $2$remaining.
</li>

<li>
In the morning of day $3$, $3$eggs are purchased. The restaurant has $2$eggs stocked on day $2$and $3$eggs stocked on day $3$.
</li>

<li>
At noon on day $3$, $2$eggs are used. The restaurant has $3$eggs stocked on day $3$remaining.
</li>

<li>
In the evening of day $3$, no eggs are discarded. (This is because all eggs stocked on day $2$have already been used.) The restaurant has $3$eggs stocked on day $3$remaining.
</li>

</ul>

<p>
Thus, $3$eggs remain after the evening action on day $3$, so output $3$on the first line.
</p>

<p>
For the second test case, remember to output the number of eggs after discarding the eggs stocked on day $1$in the evening of day $3$.
</p>

</section>

</div>

</span>

</span>

</div>
