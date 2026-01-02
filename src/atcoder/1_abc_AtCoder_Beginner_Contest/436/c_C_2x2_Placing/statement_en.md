
<div>

<span>

<span>

<p>
Score : $300$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a grid with $N$rows and $N$columns.
Let $(i,j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.
Initially, nothing is placed on the grid.
</p>

<p>
You will now perform $M$operations. The $i$-th operation $(1\leq i\leq M)$is as follows:
</p>

<ul>

<li>
Place a block that occupies a $2 \times 2$region with cell $(R_i,C_i)$as the top-left corner on the grid if and only if its position does not overlap with any other blocks already placed.
More precisely, for the set of cells $S=\lbrace (R_i,C_i),(R_i+1,C_i),(R_i,C_i+1),(R_i+1,C_i+1)\rbrace$, if there exists a block already placed on the grid that occupies any cell in $S$, do nothing;
otherwise, place a block that occupies all four cells in $S$.
</li>

</ul>

<p>
After performing all operations, find how many blocks are placed on the grid.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2\leq N \leq 10^9$
</li>

<li>
$1\leq M \leq 2\times 10^5$
</li>

<li>
$1\leq R_i,C_i \leq N-1$
</li>

<li>
All input values are integers.
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

$N$$M$$R_1$$C_1$$R_2$$C_2$$\vdots$$R_M$$C_M$
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

4 3
1 1
2 2
2 3

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
The following diagram shows the operations, where black-filled regions represent blocks and red-framed regions represent where the next block is to be placed.
</p>

<p>

<img src="https://img.atcoder.jp/abc436/1b753f2091cbd846ec88f1b0f49144cf.png">

</img>

</p>

<ul>

<li>
Operation $1$: Nothing is placed in the $2 \times 2$region with cell $(1,1)$as the top-left corner, so place a block there.
</li>

<li>
Operation $2$: Among the $2 \times 2$region with cell $(2,2)$as the top-left corner, there is already another block on cell $(2,2)$, so do nothing.
</li>

<li>
Operation $3$: Nothing is placed in the $2 \times 2$region with cell $(2,3)$as the top-left corner, so place a block there.
</li>

</ul>

<p>
Thus, after performing all operations, two blocks are placed on the grid.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

1000000000 4
1 1
1 101
101 1
101 101

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

4

</div>

<p>
Blocks can be placed in all operations.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

8 10
6 5
7 3
6 7
3 4
4 2
3 7
1 3
7 4
6 1
6 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

8

</div>

<p>
There may exist $i,j\ (i\neq j)$such that $(R_i,C_i)=(R_j,C_j)$.
</p>

</section>

</div>

</span>

</span>

</div>
