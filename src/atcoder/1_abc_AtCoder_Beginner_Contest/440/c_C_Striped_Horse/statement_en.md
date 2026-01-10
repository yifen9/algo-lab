
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
Ringo-san is trying to paint a horse with stripes to make it a zebra.
</p>

</blockquote>

<p>
There are $N$squares numbered $1$to $N$arranged in a line.

Initially, all squares are white, and the cost of painting square $i$black is $C_i$.
</p>

<p>
Consider performing the following procedure once to paint some squares black:
</p>

<ul>

<li>
Choose a positive integer $x$freely.
</li>

<li>
Paint square $i$black for all integers $i$satisfying $1 \leq i \leq N$such that the remainder when $(i+x)$is divided by $2W$is less than $W$.
</li>

</ul>

<p>
Find the minimum total cost to perform this procedure.
</p>

<p>
You are given $T$test cases; solve each of them.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T \leq 2\times 10^5$
</li>

<li>
$1\leq N \leq 2\times 10^5$
</li>

<li>
$1\leq W \leq 2\times 10^5$
</li>

<li>
$1\leq C_i \leq 10^9$
</li>

<li>
The sum of $N$over the $T$test cases is at most $2\times 10^5$.
</li>

<li>
The sum of $W$over the $T$test cases is at most $2\times 10^5$.
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
The input is given from Standard Input in the following format, where $\mathrm{case}_i$denotes the $i$-th test case.
</p>

<div>

$T$$\mathrm{case}_1$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$W$$C_1$$\dots$$C_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line should contain the answer for the $i$-th test case.
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
8 2
1 10 10 1 1 10 10 1
8 3
1 10 10 1 1 10 10 1
8 4
1 10 10 1 1 10 10 1
4 100
100000 100000 100000 100000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4
12
22
0

</div>

<p>
In the first test case, if the procedure is executed with $x=4$, squares $1,4,5,8$are painted black, and the total cost is $4$.
The total cost cannot be less than $4$, so this is the minimum.
</p>

</section>

</div>

</span>

</span>

</div>
