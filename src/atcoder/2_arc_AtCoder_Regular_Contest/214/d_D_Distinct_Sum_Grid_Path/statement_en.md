
<div>

<span>

<span>

<p>
Score : $700$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is an $N \times N$grid. Let $(i,j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.
</p>

<p>
Output one way to write a non-negative integer in each cell so that the following condition is satisfied.
</p>

<blockquote>

<p>
For a path from cell $(1,1)$to cell $(N,N)$by repeating moves only to adjacent cells to the right or down, let the 
<strong>
score
</strong>
of the path be the sum of the integers written in the cells on the path (including the start and end points).

Then, for all $\binom{2N-2}{N-1}$possible paths, the scores are all distinct and all at most $6 \times 10^6$.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 13$
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
For a way of writing that satisfies the condition in the problem statement, let $A_{i,j}$be the non-negative integer written in cell $(i,j)$, and output it in the following format:
</p>

<div>

$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,N}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,N}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,N}$
</div>

<p>
If there are multiple solutions, any of them will be accepted.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

1 2
3 4

</div>

<p>
The score of the path that moves right then down is $7$, and the score of the path that moves down then right is $8$, satisfying the condition in the problem statement.
</p>

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

10443 257776 131299 258759 153153
103533 63158 120370 132605 22808
206213 155047 237224 121264 96487
213665 51789 237311 239387 27085
229301 125534 154776 40898 210765

</div>

</section>

</div>

</span>

</span>

</div>
