
<div>

<span>

<span>

<p>
Score : $200$points
</p>

<div>

<section>

### **Problem Statement**

<p>
You are given an odd number $N$that is at least $3$.
</p>

<p>
There is a grid with $N$rows and $N$columns, where all cells are initially empty.
Now, you will write integers in each cell of this grid according to the following procedure.
Let $(i,j)$denote the cell at the $(i+1)$-th row from the top and $(j+1)$-th column from the left ($0\leq i<N, 0\leq j<N$).
</p>

<ol>

<li>
Write $1$in cell $(0,\frac{N-1}{2})$.
</li>

<li>
Repeat the following operation $N^2-1$times:
<ul>

<li>
Let $(r,c)$be the cell where an integer was written last time, and $k$be the integer written. If cell $((r-1) \bmod N, (c+1) \bmod N)$is empty, write $k+1$in that cell; otherwise, write $k+1$in cell $((r+1) \bmod N,c)$.
Here, $x \bmod N$denotes the remainder when $x$is divided by $N$.
</li>

</ul>

</li>

</ol>

<p>
Find the integer that will be written in each cell in this procedure.
It can be proved that each cell will have an integer written in it exactly once.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$3\leq N \leq 99$
</li>

<li>
$N$is an odd number.
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

$N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Let $a_{i,j}$be the integer written in cell $(i,j)$, and print it in the following format:
</p>

<div>

$a_{0,0}$$a_{0,1}$$\dots$$a_{0,N-1}$$\vdots$$a_{N-1,0}$$a_{N-1,1}$$\dots$$a_{N-1,N-1}$
</div>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

8 1 6
3 5 7
4 9 2

</div>

<p>
Integers are written in each cell as follows:
</p>

<ol>

<li>
Write $1$in cell $(0,\frac{3-1}{2})=(0,1)$.
</li>

<li>
Cell $((0-1) \bmod 3, (1+1) \bmod 3)=(2,2)$is empty, so write $2$there.
</li>

<li>
Cell $((2-1) \bmod 3, (2+1) \bmod 3)=(1,0)$is empty, so write $3$there.
</li>

<li>
Cell $((1-1) \bmod 3, (0+1) \bmod 3)=(0,1)$is not empty, so write $4$in cell $((1+1) \bmod 3,0)=(2,0)$.
</li>

<li>
$\vdots$
</li>

</ol>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

5

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

17 24 1 8 15
23 5 7 14 16
4 6 13 20 22
10 12 19 21 3
11 18 25 2 9

</div>

</section>

</div>

</span>

</span>

</div>
