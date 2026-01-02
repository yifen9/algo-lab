
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
There are $N$cells arranged in a row from left to right.

The $i$-th cell from the left $(1\leq i\leq N)$is called cell $i$.

Initially, all cells are painted white.
</p>

<p>
Process $Q$queries in order.

The $i$-th query $(1\leq i\leq Q)$is as follows:
</p>

<blockquote>

<p>
Two integers $(L_i,R_i)$$(1\leq L_i\leq R_i\leq N)$are given.

Paint all cells $L_i, L_i+1, \ldots, R_i$black.

Here, cells that were painted white are now painted black, and cells that were painted black remain as is.

After that, find the number of cells (among the $N$cells) that are painted 
<strong>
white
</strong>
.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq N\leq 10^9$
</li>

<li>
$1\leq Q\leq 2\times 10^5$
</li>

<li>
$1\leq L_i\leq R_i\leq N$
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

$N$$Q$$L_1$$R_1$$L_2$$R_2$$\vdots$$L_Q$$R_Q$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $Q$lines.

The $i$-th line $(1\leq i\leq Q)$should contain the answer to the $i$-th query.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

10 5
3 5
8 9
5 8
2 9
6 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

7
5
3
2
2

</div>

<p>
Initially, $10$cells are arranged in a row from left to right.
</p>

<ul>

<li>
The first query paints cells $3,4,5$black. After the operation, the cells painted white are cells $1,2,6,7,8,9,10$, which is $7$cells.
</li>

<li>
The second query paints cells $8,9$black. After the operation, the cells painted white are $1,2,6,7,10$, which is $5$cells.
</li>

<li>
The third query paints cells $5,6,7,8$black. After the operation, the cells painted white are $1,2,10$, which is $3$cells.
</li>

<li>
The fourth query paints cells $2,3,\ldots,9$black. After the operation, the cells painted white are $1,10$, which is $2$cells.
</li>

<li>
The fifth query paints cell $6$black. After the operation, the cells painted white are cells $1,10$, which is $2$cells.
</li>

</ul>

<p>
Thus, output $7,5,3,2,2$in this order on each line.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1000000000 1
1 500000000

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

500000000

</div>

</section>

</div>

</span>

</span>

</div>
