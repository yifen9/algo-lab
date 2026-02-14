
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
There is a grid with $N$rows and $N$columns.
The cell at the $i$-th row from the top $(1 \le i \le N)$and the $j$-th column from the left $(1 \le j \le N)$is called cell $(i,j)$.
</p>

<p>
Each cell is an empty cell or a wall cell, represented by a sequence of $N$strings of length $N$each, $(S_1,S_2,\ldots,S_N)$.
Cell $(i,j)\ (1 \le i \le N,1 \le j \le N)$is an empty cell if the $j$-th character of $S_i$is `.`, and a wall cell if it is `#`.
</p>

<p>
You want to place as many pieces as possible on this grid.
The placement of pieces is subject to the following constraints.
</p>

<ul>

<li>
A piece cannot be placed on a wall cell.
</li>

<li>
At most one piece can be placed on a single cell.
</li>

<li>
If a piece is placed on cell $(i,j)$, no piece can be placed on the cell reached by moving $A$cells vertically and $B$cells horizontally from cell $(i,j)$, or the cell reached by moving $B$cells vertically and $A$cells horizontally. More formally, if a piece is placed on cell $(i,j)$, then no piece can be placed on any of cell $(i+A,j+B),$cell $(i+B,j+A),$cell $(i+B,j-A),$cell $(i+A,j-B),$cell $(i-A,j-B),$cell $(i-B,j-A),$cell $(i-B,j+A),$cell $(i-A,j+B)$(if those cells exist).
</li>

</ul>

<p>
Let $K$be the maximum number of pieces that can be placed under these constraints, and find one placement of $K$pieces satisfying the constraints.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 300$
</li>

<li>
$0 \le A \le B \le N$
</li>

<li>
$1 \le B$
</li>

<li>
$N,A,B$are integers.
</li>

<li>
$S_i$is a string of length $N$consisting of `.`and `#`$(1 \le i \le N)$.
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

$N$$A$$B$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Find one placement of $K$pieces satisfying the constraints, and output it as strings over $N$lines.
The $i$-th line $(1 \le i \le N)$should contain a string of $N$characters consisting of `.`, `o`, and `#`.
The $j$-th character $(1 \le j \le N)$of the string on the $i$-th line should be `.`if cell $(i,j)$is an empty cell with no piece, `o`if cell $(i,j)$is an empty cell with a piece, and `#`if cell $(i,j)$is a wall cell.
</p>

<p>
If there are multiple valid placements, any of them will be accepted.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

5 1 2
..#..
..##.
.#..#
##..#
.#...

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

o.#.o
oo##.
o#..#
##.o#
o#ooo

</div>

<p>
For example, $10$pieces can be placed as follows while satisfying the constraints.
</p>

<p>

<img src="https://img.atcoder.jp/abc445/1641a8d0bdde78a148f3f782d868eab9.png">

</img>

</p>

<p>
It is impossible to place $11$pieces while satisfying the constraints, so outputting the board corresponding to the placement above,
</p>

<div>

o.#.o
oo##.
o#..#
##.o#
o#ooo

</div>

<p>
will be judged as correct.
</p>

<p>
Note that any valid placement will be accepted if there are multiple of them.
For example, the following also allows $10$pieces to be placed while satisfying the constraints.
</p>

<p>

<img src="https://img.atcoder.jp/abc445/c38f0b19c5744eefce9761819cdcd203.png">

</img>

</p>

<p>
Thus, outputting
</p>

<div>

oo#oo
o.##o
.#..#
##..#
o#ooo

</div>

<p>
will also be judged as correct.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 0 1
.###
##.#
#.##
###.

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

o###
##o#
#o##
###o

</div>

<p>
The constraints can be satisfied by placing one piece on each empty cell.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

20 3 4
#...#...........##.#
..##........#.......
.....##..#....###.#.
.#...##.##.#.#.#..#.
#...#.....###..#...#
#...##......##.##.#.
.#....#.##.##...#...
#..##..........#...#
##.#..........##....
...#..#....#.#.#...#
#.....#.##.#...#....
##................#.
.#....#..#....#.....
........#........#.#
........#.#..##....#
.##.....#....#......
.##.#.##....#.#...##
......#...#..#......
.........##...#..#.#
###.....#...#....#..

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

#ooo#....ooo....##o#
oo##o...oooo#..ooooo
ooooo##oo#ooo.###o#o
o#ooo##.##o#o#.#oo#o
#ooo#....o###..#ooo#
#...##...oo.##.##o#.
.#o...#.##.##...#oo.
#.o##.....o....#..o#
##o#.....o.o..##oo..
ooo#oo#.ooo#.#.#ooo#
#oooo.#o##o#oo.#oooo
##ooo...oooo..o.oo#o
.#oo..#o.#oo..#oooo.
........#.o......#o#
..oo....#.#o.##..o.#
.##.o...#.o..#....o.
.##o#.##...o#.#.oo##
oooooo#.oo#oo#o.oooo
.oooo..o.##ooo#oo#o#
###oooo.#ooo#.o.o#oo

</div>

</section>

</div>

</span>

</span>

</div>
