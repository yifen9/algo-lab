
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
There is an $N \times N$grid. The cell at the $i$-th row from the top and $j$-th column from the left is called $(i,j)$.

The grid is described by $N$strings $S_1,S_2,\dots,S_N$. If the $j$-th character of $S_i$is `.`, $(i,j)$is an empty cell; if it is `#`, $(i,j)$is a wall cell.
</p>

<p>
Initially, Takahashi-kun is at empty cell $(N,C)$, and repeats the following movement $N-1$times:
</p>

<ul>

<li>
If he is currently at $(r,c)$, he specifies one of $(r-1,c-1),(r-1,c),(r-1,c+1)$as the destination. Here, he cannot specify a cell that does not exist in the grid as the destination.
</li>

<li>
If the destination $(a,b)$is a wall cell, the following occurs:
<ul>

<li>
If $(i,b)$is currently an empty cell for all integers satisfying $a < i \le N$, he destroys the wall at $(a,b)$and moves there. That is, $(a,b)$becomes an empty cell and he moves to $(a,b)$.
</li>

<li>
Otherwise, he fails to move. In this case, he immediately ends the repetition of movements, even if he has not made $N-1$movements.
</li>

</ul>

</li>

<li>
If the destination $(a,b)$is an empty cell, he moves to $(a,b)$.
</li>

</ul>

<p>
Output a string $R$of length $N$satisfying the following conditions:
</p>

<ul>

<li>
If he can reach $(1,i)$without failing during the movements, the $i$-th character of $R$is `1`.
</li>

<li>
Otherwise, the $i$-th character of $R$is `0`.
</li>

</ul>

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
$T,N,C$are integers.
</li>

<li>
$1 \le T \le 50000$
</li>

<li>
$2 \le N \le 3000$
</li>

<li>
$1 \le C \le N$
</li>

<li>
$S_i$is a string of length $N$consisting of `.`and `#`.
</li>

<li>
The $C$-th character of $S_N$is `.`.
</li>

<li>
For each input, the sum of $N^2$does not exceed $9 \times 10^6$.
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

$N$$C$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Print $T$lines.
</p>

<p>
The $i$-th line should contain the answer for the $i$-th test case.
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
5 3
.###.
..#..
#.#.#
#...#
##..#
2 2
##
..
4 1
####
####
####
.###
3 3
...
...
...
10 3
##.##.##.#
.####..#..
...#.#..#.
.#.#.#.#..
...####...
#.#.##....
.##...#...
#.##.....#
#....###.#
.#..#.#...

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

10111
11
1000
111
0011010010

</div>

<p>
This input contains five test cases.
</p>

<p>
For the first test case, for example, he can reach $(1,3)$without failing during the movements as follows:
</p>

<ul>

<li>
Initially, he is at $(5,3)$.
</li>

<li>
He moves to empty cell $(4,2)$.
</li>

<li>
$(3,3)$is a wall cell, but since $(4,3),(5,3)$are currently both empty cells, he destroys the wall at $(3,3)$and moves to $(3,3)$.
</li>

<li>
$(2,3)$is a wall cell, but since $(3,3),(4,3),(5,3)$are currently all empty cells, he destroys the wall at $(2,3)$and moves to $(2,3)$.
</li>

<li>
$(1,3)$is a wall cell, but since $(2,3),(3,3),(4,3),(5,3)$are currently all empty cells, he destroys the wall at $(1,3)$and moves to $(1,3)$.
</li>

</ul>

<p>
He can reach $(1,1),(1,3),(1,4),(1,5)$without failing during the movements, so print `10111`.
</p>

</section>

</div>

</span>

</span>

</div>
