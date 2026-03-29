
<div>

<span>

<span>

<p>
Score : $1000$points
</p>

<div>

<section>

### **Problem Statement**

<blockquote>

<p>
Consider writing $0$or $1$on each vertex of a $4\times 500$grid graph. Write the values cleverly so that for each $N=0,1,\ldots,999899,999900$, the following condition is satisfied.

</p>

<ul>

<li>
There exists a Hamiltonian path on the grid graph such that the sequence of numbers written on the vertices along the path has an inversion count of $N$.
</li>

</ul>

<img src="https://img.atcoder.jp/agc077/f8959792e6ca2bd80a2a8a9a018dcf8a.gif">

</img>

<p>
An example with $3\times 4$. With this assignment, $N = 10, 11, \ldots, 20$are achievable.
</p>

<p>

</p>

</blockquote>

---

<p>
This is an 
<strong>
interactive
</strong>
problem. 
<strong>
The parameters in the problem statement are fixed at $H=4,W=500,Q=200$.
</strong>

</p>

<p>
You and the judge perform the following steps. The steps consist of Phase $1$and Phase $2$; Phase $1$is performed first, immediately followed by Phase $2$.
</p>

<p>
(Phase $1$)
</p>

<p>
Output an $H\times W$matrix $A=(A_{i,j})\ (1\leq i\leq H,1\leq j\leq W)$where each element is $0$or $1$.
</p>

<p>
(Phase $2$)
</p>

<p>
Solve the following problem $Q$times.
</p>

<blockquote>

<p>
The judge gives you an integer $N$.

Consider an $H$-row $W$-column grid. The cell $(i,j)$, located at the $i$-th row from the top and the $j$-th column from the left, has the integer $A_{i,j}$written on it.

Find a path $P$of length $HW$that starts at any cell, moves to an adjacent cell (up, down, left, or right) repeatedly, visits all $HW$cells exactly once, and ends at any cell, such that the following is satisfied.

</p>

<ul>

<li>
The inversion count of the sequence of length $HW$obtained by listing the integers written on the cells visited by $P$in order is $N$.
</li>

</ul>

<p>

</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$H=4,W=500,Q=200$
</li>

<li>
$0\leq N\leq 999900$
</li>

<li>
All input values are integers.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Interaction**

<p>
This is an interactive problem.
</p>

<p>
First, $H,W,Q$are given from Standard Input.
</p>

<div>

$H$$W$$Q$
</div>

<p>
(Phase $1$)
</p>

<p>
Output an $H\times W$matrix $A=(A_{i,j})\ (1\leq i\leq H,1\leq j\leq W)$where each element is $0$or $1$, over $H$lines.
</p>

<p>
The $i$-th line should contain $A_{i,1}A_{i,2}\ldots A_{i,W}$as a string of length $W$consisting of `0`and `1`.
</p>

<div>

$A_{1,1}A_{1,2}\ldots A_{1,W}$$A_{2,1}A_{2,2}\ldots A_{2,W}$$\vdots$$A_{H,1}A_{H,2}\ldots A_{H,W}$
</div>

<p>
(Phase $2$)
</p>

<p>
Solve the problem $Q$times. For each problem, first an integer $N$is given from Standard Input.
</p>

<div>

$N$
</div>

<p>
(Note: if your answer to the previous problem was incorrect, or if $A$or the path was output in an incorrect format, then instead of $N$, `-1`is given from Standard Input here. In that case, immediately terminate the program normally. However, if an incorrect output is given for the first time in the $Q$-th problem, no further input will be given.)
</p>

<p>
Then, output a path $P$satisfying the condition, where the $i$-th visited cell is $(x_i, y_i)$, in the following format:
</p>

<div>

$x_1$$y_1$$x_2$$y_2$$\vdots$$x_{HW}$$y_{HW}$
</div>

<p>
$x_i$and $y_i$must satisfy the following.
</p>

<ul>

<li>
$1\leq x_i\leq H, 1\leq y_i\leq W$.
</li>

<li>
$(x_i,y_i)\neq (x_j,y_j)$if $i\neq j$.
</li>

<li>
$|x_i-x_{i+1}|+|y_i-y_{i+1}|=1$for $i=1,2,\ldots,HW-1$.
</li>

<li>
The inversion count of the sequence $(A_{x_1,y_1}, A_{x_2,y_2},\ldots,A_{x_{HW},y_{HW}})$is $N$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Notes**

<ul>

<li>

<b>

<span>
If you receive `-1`as input from the judge, immediately terminate the program normally. If you terminate, the verdict will be 
<span>
WA
</span>
; otherwise, the verdict is indeterminate.
</span>

</b>

</li>

<li>

<strong>
In each output, include a newline at the end and flush Standard Output. Otherwise, the verdict may be 
<span>
TLE
</span>
.
</strong>

</li>

<li>

<strong>
Extra newlines in output are considered as malformed; do not include them.
</strong>

</li>

<li>
Terminate your program immediately after finishing Phase $2$. Otherwise, the verdict is indeterminate.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Sample Interaction**

<p>
Below is a sample interaction for the case $H=3,W=4,Q=2$.
</p>

<p>
This example does not satisfy the constraints and is not included in the judge.
</p>

<table>

<colgroup>

<col>

</col>

<col>

</col>

<col>

</col>

</colgroup>

<thead>

<tr>

<th>
Input
</th>

<th>
Output
</th>

<th>
Explanation
</th>

</tr>

</thead>

<tbody>

<tr>

<td>

<div>

3 4 2

</div>

</td>

<td>

</td>

<td>
$H,W,Q$are given.
</td>

</tr>

<tr>

<td>

</td>

<td>

<div>

1101
0110
1010

</div>

</td>

<td>
Output $A=\begin{pmatrix} 1&1&0&1 \\ 0&1&1&0 \\ 1&0&1&0 \end{pmatrix}$.
</td>

</tr>

<tr>

<td>

<div>

10

</div>

</td>

<td>

</td>

<td>
$N$for the first problem is given.
</td>

</tr>

<tr>

<td>

</td>

<td>

<div>

3 2
3 3
3 4
2 4
1 4
1 3
2 3
2 2
1 2
1 1
2 1
3 1

</div>

</td>

<td>
Output the path $(3,2)\to(3,3)\to(3,4)\to(2,4)\to(1,4)\to(1,3)\to(2,3)\to(2,2)\to(1,2)\to(1,1)\to(2,1)\to(3,1)$. The sequence of integers written on the cells visited along this path is $(0,1,0,0,1,0,1,1,1,1,0,1)$, and the inversion count of this sequence is $10$, so the condition is satisfied.
</td>

</tr>

<tr>

<td>

<div>

15

</div>

</td>

<td>

</td>

<td>
$N$for the second problem is given.
</td>

</tr>

<tr>

<td>

</td>

<td>

<div>

1 1
2 1
3 1
3 2
3 3
3 4
2 4
2 3
2 2
1 2
1 3
1 4

</div>

</td>

<td>
Output the path $(1,1)\to(2,1)\to(3,1)\to(3,2)\to(3,3)\to(3,4)\to(2,4)\to(2,3)\to(2,2)\to(1,2)\to(1,3)\to(1,4)$. The sequence of integers written on the cells visited along this path is $(1, 0, 1, 0, 1, 0, 0, 1, 1, 1, 0, 1)$, and the inversion count of this sequence is $15$, so the condition is satisfied.
</td>

</tr>

</tbody>

</table>

</section>

</div>

</span>

</span>

</div>
