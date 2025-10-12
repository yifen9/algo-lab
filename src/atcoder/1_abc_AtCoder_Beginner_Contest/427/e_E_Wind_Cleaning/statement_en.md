
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
There is a grid with $H$rows and $W$columns. Let $(i, j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.
</p>

<p>
Takahashi is on one of the cells in this grid, and there is trash on some cells of the grid.
</p>

<p>
The states of the cells are given by $H$strings $S_1, S_2, \ldots, S_H$of length $W$, where $S_{i, j}$denotes the $j$-th character of $S_i$and represents the following state:
</p>

<ul>

<li>
If $S_{i, j} =$`T`, cell $(i, j)$is the cell where Takahashi is.
</li>

<li>
If $S_{i, j} =$`#`, cell $(i, j)$is a cell with trash.
</li>

<li>
If $S_{i, j} =$`.`, cell $(i, j)$is an empty cell without trash.
</li>

</ul>

<p>
There is no trash on the cell where Takahashi is.
</p>

<p>
He can repeatedly perform the following operation:
</p>

<ul>

<li>
Choose one of the four directions (up, down, left, or right), and move all trash simultaneously one cell in that direction. Here, if trash goes outside the grid, the trash disappears, and if trash moves to the cell where he is, he gets dirty.
</li>

</ul>

<p>
Determine whether it is possible for him to make all trash disappear without getting dirty, and if possible, find the minimum possible number of operations.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \leq H, W \leq 12$
</li>

<li>
$S_i$is a string of length $W$consisting of `T`, `#`, and `.`.
</li>

<li>
There is exactly one $(i, j)$such that $S_{i, j} =$`T`.
</li>

<li>
There is at least one $(i, j)$such that $S_{i, j} =$`#`.
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

$H$$W$$S_1$$S_2$$\vdots$$S_H$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible for Takahashi to make all trash disappear without getting dirty, print the minimum possible number of operations. Otherwise, print `-1`.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 4
###.
#.T.
...#

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3

</div>

<p>
Takahashi can make all trash disappear in three operations as follows:
</p>

<ul>

<li>

<p>
Choose up. After this operation, trash is on cells $(1, 1)$and $(2, 4)$. 
</p>

</li>

<li>

<p>
Choose right. After this operation, trash is on cell $(1, 2)$.
</p>

</li>

<li>

<p>
Choose up. After this operation, all trash has disappeared.
</p>

</li>

</ul>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 3
###
#T#
###

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

5 5
###..
#T...
..##.
##..#
#..#.

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
