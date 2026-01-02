
<div>

<span>

<span>

<p>
Score : $600$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is an $N \times N$grid. The cell at the $i$-th row from the top and $j$-th column from the left is called $(i,j)$.
</p>

<p>
For each way of writing $0$or $1$in each cell, define $f(X)$as follows:
</p>

<ul>

<li>
The number of ways to move from a cell with $X$written on it to another cell with $X$written on it by repeating the operation "move to the right adjacent cell or move to the down adjacent cell" 
<strong>
one or more times
</strong>
.
</li>

</ul>

<p>
Construct one way of writing that satisfies $f(0) = f(1)$. It is guaranteed that a solution exists under the constraints of this problem.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 500$
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

$N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines. The $i$-th line $(1 \le i \le N)$should contain the digits to be written in $(i,1),(i,2),\dots,(i,N)$in this order without spaces.
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

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

01
01

</div>

<p>
There is one way, shown below, to perform operations satisfying the condition for $f(0)$, so $f(0) = 1$.
</p>

<ul>

<li>
Start from $(1,1)$and move to $(2,1)$.
</li>

</ul>

<p>
There is one way, shown below, to perform operations satisfying the condition for $f(1)$, so $f(1) = 1$.
</p>

<ul>

<li>
Start from $(1,2)$and move to $(2,2)$.
</li>

</ul>

<p>
Since $f(0) = f(1)$, the condition is satisfied.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

100111
101000
100010
011101
010000
110001

</div>

</section>

</div>

</span>

</span>

</div>
