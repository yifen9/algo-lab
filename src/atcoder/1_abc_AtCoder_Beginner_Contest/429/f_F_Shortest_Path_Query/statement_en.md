
<div>

<span>

<span>

<p>
Score : $525$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given a grid with three rows and $N$columns. Denote the cell at the $i$-th row from the top and $j$-th column from the left as cell $(i,j)$. Cell $(i,j)$is a wall cell if $S_{i,j}$is `#`, and an empty cell and passable if it is `.`.
</p>

<p>
You are given $Q$queries, which you should process in order.
</p>

<p>
Each query gives integers $r$and $c$, and you should flip the state of cell $(r,c)$. That is, if cell $(r,c)$is a wall cell, make it an empty cell, and if it is an empty cell, make it a wall cell. Then, output the answer to the following problem:
</p>

<blockquote>

<p>
Consider moving from cell $(1,1)$to cell $(3,N)$by repeatedly moving to an empty cell adjacent up, down, left, or right. Determine whether cell $(3,N)$is reachable, and if reachable, find the minimum number of moves.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\le N\le 2\times 10^5$
</li>

<li>
$S_{i,j}$is `#`or `.`.
</li>

<li>
$S_{1,1}=S_{3,N}=$`.`
</li>

<li>
$1\le Q\le 2\times 10^5$
</li>

<li>
$1\le r\le 3$
</li>

<li>
$1\le c\le N$
</li>

<li>
$(r,c) \neq (1,1),(3,N)$
</li>

<li>
$N,Q,r,c$are integers.
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

$N$$S_{1,1}S_{1,2}\ldots S_{1,N}$$S_{2,1}S_{2,2}\ldots S_{2,N}$$S_{3,1}S_{3,2}\ldots S_{3,N}$$Q$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
Each query is given in the following format:
</p>

<div>

$r$$c$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $Q$lines.
</p>

<p>
On the $i$-th line $(1\le i\le Q)$, if cell $(3,N)$is unreachable from cell $(1,1)$in the $i$-th query, print `-1`; if reachable, print the minimum number of moves.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5
.#...
.#.#.
...#.
3
1 2
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

6
10
-1

</div>

<p>
In the first query, flip the state of cell $(1,2)$. As a result, the state of each cell becomes:
</p>

<div>

.....
.#.#.
...#.

</div>

<p>
At this time, by moving from cell $(1,1)$through cells $(1,2),(1,3),(1,4),(1,5),(2,5),(3,5)$in order, you can reach cell $(3,5)$in six moves.
</p>

<p>
In the second query, flip the state of cell $(1,2)$. As a result, the state of each cell becomes:
</p>

<div>

.#...
.#.#.
...#.

</div>

<p>
At this time, by moving from cell $(1,1)$through cells $(2,1),(3,1),(3,2),(3,3),(2,3),(1,3),(1,4),(1,5),(2,5),(3,5)$in order, you can reach cell $(3,5)$in ten moves.
</p>

<p>
In the third query, flip the state of cell $(2,3)$. As a result, the state of each cell becomes:
</p>

<div>

.#...
.###.
...#.

</div>

<p>
At this time, no matter how you move, you cannot reach cell $(3,5)$from cell $(1,1)$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

7
.#.....
.#..#..
...#...
6
2 5
3 4
3 5
2 5
1 4
1 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

10
8
10
12
-1
12

</div>

</section>

</div>

</span>

</span>

</div>
