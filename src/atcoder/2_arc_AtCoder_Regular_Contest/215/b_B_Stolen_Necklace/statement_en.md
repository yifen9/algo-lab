
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $2N$gems arranged in a row from left to right, and the type of the $i$-th gem from the left is $A_i$. Here, $A_i$is an integer between $1$and $N$, inclusive, and there are exactly two gems of each type.
</p>

<p>
You want to insert dividers satisfying the following conditions.
</p>

<ul>

<li>
Each divider's position is represented by an integer $i$($1 \le i \le 2N - 1$), meaning it divides between the $i$-th and $(i+1)$-th gems from the left.
</li>

<li>
No two or more dividers exist at the same position.
</li>

<li>
The number of dividers $K$is at most $N$.
</li>

<li>
Inserting $K$dividers divides the row of gems into $K + 1$segments. Here, collecting all gems in the odd-numbered (first, third, ...) segments from the left yields exactly one gem of each type $1, 2, \ldots, N$.
</li>

</ul>

<p>
Output one way to insert dividers satisfying this condition. It can be proved that such a way always exists.
</p>

<p>
You are given $T$test cases; solve each one.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le T \le 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i \le N$($1 \le i \leq 2N$)
</li>

<li>
There are exactly two gems of each type. That is, for each $x$($1 \le x \le N$), there are exactly two indices $i$with $A_i = x$.
</li>

<li>
The sum of $N$over all test cases is at most $2 \times 10^5$.
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$N$$A_1$$A_2$$\ldots$$A_{2N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output for the $T$test cases in order.
</p>

<p>
For each test case, output a way to insert dividers satisfying the condition.
Specifically, let $K$be the number of dividers and $C_1, C_2, \ldots, C_K$be the positions of the dividers in ascending order, and output in the following format:
</p>

<div>

$K$$C_1$$C_2$$\ldots$$C_K$
</div>

<p>
Here, $K$must be at most $N$. 
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2
3
1 2 2 3 3 1
5
1 2 3 4 5 5 4 3 2 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3
1 2 4
1
5

</div>

<p>
For the first test case, inserting dividers at positions $1, 2, 4$divides the gems into segments $(1),(2),(2,3),(3,1)$, and collecting all gems in the odd-numbered segments from the left yields exactly one gem of each type $1, 2, 3$.
</p>

</section>

</div>

</span>

</span>

</div>
