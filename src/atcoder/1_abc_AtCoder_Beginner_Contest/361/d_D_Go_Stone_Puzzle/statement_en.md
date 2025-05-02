
<div>

<span>

<span>

<p>
Score : $425$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There are $N+2$cells arranged in a row. Let cell $i$denote the $i$-th cell from the left.
</p>

<p>
There is one stone placed in each of the cells from cell $1$to cell $N$.

For each $1 \leq i \leq N$, the stone in cell $i$is white if $S_i$is `W`, and black if $S_i$is `B`.

Cells $N+1$and $N+2$are empty.
</p>

<p>
You can perform the following operation any number of times (possibly zero):
</p>

<ul>

<li>
Choose a pair of adjacent cells that both contain stones, and move these two stones to the empty two cells while preserving their order.

More precisely, choose an integer $x$such that $1 \leq x \leq N+1$and both cells $x$and $x+1$contain stones. Let $k$and $k+1$be the empty two cells. Move the stones from cells $x$and $x+1$to cells $k$and $k+1$, respectively.
</li>

</ul>

<p>
Determine if it is possible to achieve the following state, and if so, find the minimum number of operations required:
</p>

<ul>

<li>
Each of the cells from cell $1$to cell $N$contains one stone, and for each $1 \leq i \leq N$, the stone in cell $i$is white if $T_i$is `W`, and black if $T_i$is `B`.  
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 14$
</li>

<li>
$N$is an integer.
</li>

<li>
Each of $S$and $T$is a string of length $N$consisting of `B`and `W`.
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

$N$$S$$T$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible to achieve the desired state, print the minimum number of operations required. If it is impossible, print `-1`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

6
BWBWBW
WWWBBB

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4

</div>

<p>
Using `.`to represent an empty cell, the desired state can be achieved in four operations as follows, which is the minimum:
</p>

<ul>

<li>
`BWBWBW..`
</li>

<li>
`BW..BWBW`
</li>

<li>
`BWWBB..W`
</li>

<li>
`..WBBBWW`
</li>

<li>
`WWWBBB..`
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

6
BBBBBB
WWWWWW

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

14
BBBWBWWWBBWWBW
WBWWBBWWWBWBBB

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

7

</div>

</section>

</div>

</span>

</span>

</div>
