
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
We have an $N \times N$grid. Let $(i,j)$denote the square at the $i$-th row from the top and $j$-th column from the left in this grid.

Find one way to write an integer on every square to satisfy the conditions below.
</p>

<ul>

<li>
Each integer between $1$and $N^2$is written exactly once.
</li>

<li>
For every pair of integers $i,j\, (1 \leq i,j \leq N)$, the square $(i,j)$satisfies the following.
<ul>

<li>
Among the squares horizontally, vertically, or diagonally adjacent to $(i,j)$(there are at most eight of them), let $a$and $b$be the number of squares with integers larger than and smaller than that of $(i,j)$, respectively. Then, $a \neq b$holds.
</li>

</ul>

</li>

</ul>

<p>
Under the Constraints of this problem, it can be proved that such a way to write integers always exists.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq N \leq 500$
</li>

<li>
$N$is an integer.
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
Input is given from Standard Input in the following format:
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
Print a way to write integers to satisfy the conditions, in the following format:
</p>

<div>

$x_{1,1}$$\ldots$$x_{1,N}$$\vdots$$x_{N,1}$$\ldots$$x_{N,N}$
</div>

<p>
Here, $x_{i,j}$is the integer to write on the square $(i,j)$.

If multiple solutions exist, any of them will be accepted.
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

1 2
3 4

</div>

<p>
This output contains each integer between $1$and $N^2\, (=4)$exactly once, so the first condition is satisfied.

Additionally, among the squares horizontally, vertically, or diagonally adjacent to the square $(1,1)$, three squares $(1,2)$, $(2,1)$, and $(2,2)$have integers larger than that of $(1,1)$, and none has an integer smaller than that.

Thus, for $(1,1)$, we have $a=3$and $b=0$, so $a\neq b$holds.

Similarly, it can be verified that $a\neq b$also holds for the other squares, so the second condition is satisfied.

Therefore, this output is valid.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

1 2 3
5 4 6
7 8 9

</div>

</section>

</div>

</span>

</span>

</div>
