
<div>

<span>

<span>

<p>
Score : $900$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is an $H \times W$grid. Let $(i,j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.
</p>

<p>
Each cell is an empty cell or a wall cell, and this information is represented by $H \times W$characters $S_{1,1},\dots ,S_{H,W}$.
Cell $(i,j)$is an empty cell if $S_{i,j}$is `.`, and a wall cell if it is `#`.
</p>

<p>
Initially, Takahashi is at cell $(1,1)$.
He can move to a cell adjacent to his current cell in one of the four directions (up, down, left, right) any number of times.
However, 
<strong>
he cannot move in the same direction twice in a row
</strong>
.
Also, he cannot move to a wall cell or outside the grid.
</p>

<p>
Before starting to move, he can destroy zero or more wall cells to change them into empty cells.
What is the minimum number of wall cells he needs to destroy to reach cell $(H,W)$?
Under the constraints of this problem, it can be proved that there exists a way to destroy wall cells so that he can reach cell $(H,W)$.
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
$1 \le T \le 1000$
</li>

<li>
$2 \le H, W \le 100$
</li>

<li>
$S_{i,j}$is `.`or `#`.
</li>

<li>
$S_{1,1}$and $S_{H,W}$are `.`.
</li>

<li>
The sum of $HW$over all test cases is at most $3 \times 10^4$.
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

$H$$W$$S_{1,1}$$S_{1,2}$$\ldots$$S_{1,W}$$S_{2,1}$$S_{2,2}$$\ldots$$S_{2,W}$$\vdots$$S_{H,1}$$S_{H,2}$$\ldots$$S_{H,W}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines.
</p>

<p>
The $i$-th line should contain the minimum possible number of wall cells to destroy for Takahashi to reach cell $(H,W)$for the $i$-th test case.
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
3 5
..##.
.#...
##.#.
2 3
..#
#..
13 13
.############
##.##..###..#
#.#.#.#.#.###
#...#..##.###
#.#.#.#.#.###
#.#.#.#.##..#
#############
#...##.##.#.#
###.#..##.#.#
#...##.##...#
#.####.####.#
#...#...###.#
############.

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
0
13

</div>

<p>
For the first test case, Takahashi can reach cell $(H,W)$by destroying two wall cells as shown below.
</p>

<p>

<img src="https://img.atcoder.jp/arc214/78ec0e8b7eb9370afc68684193b87232.png">

</img>

</p>

<p>
The left side shows an example of wall cells to destroy, and the right side shows an example of a movement path.
Note that it is not necessary to minimize the number of moves, and it is allowed to visit the same cell more than once.
</p>

<p>
For the second test case, he can reach cell $(H,W)$without destroying any wall cells.
</p>

</section>

</div>

</span>

</span>

</div>
