
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
There is a grid with $N$rows and $N$columns. The square at the $i$-th row from the top and $j$-th column from the left is denoted as square $(i, j)$.
</p>

<p>
Each square in the grid is painted white or black. The information of the grid is given by $N$strings $S_1, S_2, \ldots, S_N$. If the $j$-th character of $S_i$is `.`, square $(i, j)$is painted white; if the $j$-th character of $S_i$is `#`, square $(i, j)$is painted black.
</p>

<p>
You will repaint some squares so that both of the following conditions are satisfied:
</p>

<ul>

<li>
For every row, the following condition holds:
<ul>

<li>
There exists an integer $k$satisfying $0 \leq k \leq N$such that the leftmost $k$squares of that row are painted white and the other squares are painted black.
</li>

</ul>

</li>

<li>
For every column, the following condition holds:
<ul>

<li>
There exists an integer $k$satisfying $0 \leq k \leq N$such that the topmost $k$squares of that column are painted white and the other squares are painted black.
</li>

</ul>

</li>

</ul>

<p>
Find the minimum number of squares that need to be repainted to satisfy the conditions.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq N \leq 5000$
</li>

<li>
$N$is an integer.
</li>

<li>
$S_i$is a string of length $N$consisting of `.`and `#`.
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

$N$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print the answer.
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
..#
#.#
.#.

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2

</div>

<p>
You can satisfy the conditions by repainting square $(2, 1)$white and square $(3, 3)$black.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5
..#.#
#..##
###.#
.###.
#....

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

9

</div>

</section>

</div>

</span>

</span>

</div>
