
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
There is an $N \times N$grid, and there is one piece placed in each column.

The piece in column $i$is placed in row $R_i$from the top.
</p>

<p>
You can perform the following operation zero or more times:
</p>

<ul>

<li>
Choose a piece that is not in the topmost row and move that piece to the 
<strong>
cell directly above it
</strong>
.
</li>

</ul>

<p>
Find the minimum number of operations needed to satisfy the following condition for all integers $i$satisfying $1 \le i \le N-1$:
</p>

<ul>

<li>
Let the piece in column $i$be in row $x$from the top and the piece in column $i+1$be in row $y$from the top. Then, $|x-y| \le 1$.
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
All input values are integers.
</li>

<li>
$1 \le T \le 50000$
</li>

<li>
$2 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le R_i \le N$
</li>

<li>
For a single input, the sum of $N$does not exceed $3 \times 10^5$.
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

$N$$R_1$$R_2$$\dots$$R_N$
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
5
5 2 1 3 4
2
1 1
3
1 3 1
9
9 9 8 2 4 4 3 5 3
20
7 4 6 2 15 5 17 15 1 8 18 1 5 1 12 11 2 7 8 14

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

4
0
1
16
105

</div>

<p>
This input contains five test cases.
</p>

<p>
For the first test case, by performing operations as follows, you can satisfy the condition in the problem statement with four operations, which is the minimum.
</p>

<ul>

<li>
Move the piece in the $5$-th column from the left to the cell directly above it. The pieces are in rows $5,2,1,3,3$from left to right.
</li>

<li>
Move the piece in the $1$-st column from the left to the cell directly above it. The pieces are in rows $4,2,1,3,3$from left to right.
</li>

<li>
Move the piece in the $1$-st column from the left to the cell directly above it. The pieces are in rows $3,2,1,3,3$from left to right.
</li>

<li>
Move the piece in the $4$-th column from the left to the cell directly above it. The pieces are in rows $3,2,1,2,3$from left to right.
</li>

</ul>

<p>
For the second test case, the condition is satisfied without performing any operations.
</p>

</section>

</div>

</span>

</span>

</div>
