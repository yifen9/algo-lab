
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
There is a maze consisting of a grid with $H$rows and $W$columns.
Let $(i,j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.
The type of cell $(i,j)$is given as a character $S_{i,j}$, where each character has the following meaning:
</p>

<ul>

<li>
`.`: Empty cell
</li>

<li>
`#`: Obstacle cell
</li>

<li>
Lowercase English letter (`a`- `z`): Warp cell
</li>

</ul>

<p>
In the maze, you can perform the following two types of actions any number of times in any order:
</p>

<ul>

<li>
Walk: Move from the current cell to a cell that is one cell away in one of the four directions (up, down, left, right). However, you cannot move to an obstacle cell or outside the grid.
</li>

<li>
Warp: When you are at a warp cell, move to any warp cell with the same character written on it.
</li>

</ul>

<p>
Determine whether it is possible to move from cell $(1,1)$to cell $(H,W)$, and if possible, find the minimum total number of actions required.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq H,W \leq 1000$
</li>

<li>
$H\times W \geq 2$
</li>

<li>
$H$and $W$are integers.
</li>

<li>
$S_{i,j}$is `.`, `#`, or a lowercase English letter.
</li>

<li>
$S_{1,1}\neq$`#`
</li>

<li>
$S_{H,W}\neq$`#`
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

$H$$W$$S_{1,1}S_{1,2}\dots S_{1,W}$$\vdots$$S_{H,1}S_{H,2}\dots S_{H,W}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is possible to move from cell $(1,1)$to cell $(H,W)$, print the minimum total number of actions required; otherwise, print `-1`.
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
..a.
####
ba#b

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

5

</div>

<p>
You can move from cell $(1,1)$to cell $(3,4)$by performing actions as follows:
</p>

<ol>

<li>
Move from cell $(1,1)$to cell $(1,2)$by walking.
</li>

<li>
Move from cell $(1,2)$to cell $(1,3)$by walking.
</li>

<li>
Move from cell $(1,3)$to cell $(3,2)$by warping. 
</li>

<li>
Move from cell $(3,2)$to cell $(3,1)$by walking. 
</li>

<li>
Move from cell $(3,1)$to cell $(3,4)$by warping.
</li>

</ol>

<p>
The total number of actions is $5$, which is the minimum.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

3 4
..a.
####
b.#b

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
It is impossible to move from cell $(1,1)$to cell $(3,4)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

4 4
xxxx
xxxx
xxxx
xxxx

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

7 11
u..#y..#...
k..#.z.#.k.
iju#...#x..
###########
..x#.t.#..n
abc#y..#...
..z#..t#.y.

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

12

</div>

</section>

</div>

</span>

</span>

</div>
