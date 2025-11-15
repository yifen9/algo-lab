
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
There is an infinitely large two-dimensional grid. The color of cell $(x,y)$is black if $0 \leq x \leq X-1$and $0 \leq y \leq Y-1$, and white otherwise.
</p>

<p>
$N$great storms occur in order on this grid. The $i$-th great storm updates the color of each cell on the grid according to a rule represented by a character $C_i$and integers $A_i, B_i$.
</p>

<p>
In the $i$-th great storm, the color of cell $(x, y)$after the great storm is:
</p>

<ul>

<li>
In case $C_i$is `X`,
<ul>

<li>
if $x <    A_i$, it becomes the color of cell $(x, y + B_i)$before the great storm;
</li>

<li>
if $x \geq A_i$, it becomes the color of cell $(x, y - B_i)$before the great storm.
</li>

</ul>

</li>

<li>
In case $C_i$is `Y`,
<ul>

<li>
if $y <    A_i$, it becomes the color of cell $(x + B_i, y)$before the great storm;
</li>

<li>
if $y \geq A_i$, it becomes the color of cell $(x - B_i, y)$before the great storm.
</li>

</ul>

</li>

</ul>

<p>
Two black cells $(x_1, y_1), (x_2, y_2)$are 
<strong>
adjacent
</strong>
if and only if $|x_1 - x_2| + |y_1 - y_2| = 1$. Also, two black cells $c_1, c_2$are 
<strong>
connected
</strong>
if and only if one can move from cell $c_1$to cell $c_2$by repeatedly moving to adjacent black cells.
</p>

<p>
A non-empty set $S$of black cells is a 
<strong>
connected component
</strong>
if and only if $S$satisfies the following conditions:
</p>

<ul>

<li>
Any two cells in $S$are connected.
</li>

<li>
Every black cell not in $S$is not connected to any cell in $S$.
</li>

</ul>

<p>
For the grid after all $N$great storms have occurred, find the number of connected components and output the number of cells in each connected component 
<strong>
in ascending order
</strong>
.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$N, X, Y$are integers.
</li>

<li>
$1 \leq N \leq 14$
</li>

<li>
$1 \leq X,Y \leq 10^8$
</li>

<li>
$C_i$is `X`or `Y`.
</li>

<li>
$A_i, B_i$are integers.
</li>

<li>
$-10^8 \leq A_i, B_i \leq 10^8$
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

$N$$X$$Y$$C_1$$A_1$$B_1$$\vdots$$C_N$$A_N$$B_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output two lines.
</p>

<p>
The first line should contain the number of connected components consisting of black cells.
</p>

<p>
The second line should contain the number of cells in each connected component, space-separated, 
<strong>
in ascending order
</strong>
.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2 3 5
X 2 2
Y -1 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2
2 13

</div>

<p>
The grid changes as shown in the following image due to the great storms (the rightward direction is the positive direction of the $x$-axis, and the upward direction is the positive direction of the $y$-axis).
</p>

<p>

<img src="https://img.atcoder.jp/abc432/6807ffb1d3c5656e1849f8c8cc06665b.png">

</img>

</p>

<p>
In the final grid, the following two connected components exist:
</p>

<ul>

<li>
A connected component consisting of cells $(-1,-2), (0,-2)$.
</li>

<li>
A connected component consisting of cells $(1,-1), (1,0), (1,1), (1,2), (2,-1), (2,0), (2,1), (2,2), (3,2), (3,3), (3,4), (3,5), (3,6)$.
</li>

</ul>

<p>
Note that the number of cells in each connected component must be output 
<strong>
in ascending order
</strong>
.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

14 68875272 94216928
X 1630731 32914676
X 17164413 -33684569
X 26798060 5418308
X 34094469 -45675954
X 43889566 34125482
X 56836569 -22217058
X 64045210 27857939
Y -54561094 11587606
Y 93548188 32214521
Y -77361096 25750481
Y 27724899 1810420
Y 80945185 -7871305
Y 14782822 -2565089
Y 54687684 -22884393

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

8
21105046168287 22050167303226 33624667752182 223328231190194 441936776830492 1141371400772596 1141702254882183 3464097998105256

</div>

<p>
The output value may not fit in a 32-bit integer.
</p>

</section>

</div>

</span>

</span>

</div>
