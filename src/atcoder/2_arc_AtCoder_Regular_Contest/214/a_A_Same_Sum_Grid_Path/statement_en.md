
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
There is an $N \times N$grid. Let $(i,j)$denote the cell at the $i$-th row from the top and $j$-th column from the left.
</p>

<p>
You are given $N \times N$characters $S_{1,1}, \dots , S_{N,N}$. Each character is a digit (`0`to `9`) or `?`. Determine if it is possible to replace each `?`with a digit to satisfy the following condition, and if possible, output one such way of replacement.
</p>

<blockquote>

<p>
For each $1 \le i,j \le N$, write $S_{i,j}$as an integer in cell $(i,j)$.

For a path from cell $(1,1)$to cell $(N,N)$by repeating moves only to adjacent cells to the right or down, let the 
<strong>
score
</strong>
of the path be the sum of the integers written in the cells on the path (including the start and end points).

Then, for all $\binom{2N-2}{N-1}$possible paths, the scores are all equal.
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$2 \le N \le 100$
</li>

<li>
$S_{i,j}$is a digit (`0`to `9`) or `?`.
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

$N$$S_{1,1}$$S_{1,2}$$\ldots$$S_{1,N}$$S_{2,1}$$S_{2,2}$$\ldots$$S_{2,N}$$\vdots$$S_{N,1}$$S_{N,2}$$\ldots$$S_{N,N}$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
If it is impossible to make a replacement that satisfies the condition, output `-1`. If possible, output $S_{1,1}, \dots , S_{N,N}$after the replacement in the following format:
</p>

<div>

$S_{1,1}$$S_{1,2}$$\ldots$$S_{1,N}$$S_{2,1}$$S_{2,2}$$\ldots$$S_{2,N}$$\vdots$$S_{N,1}$$S_{N,2}$$\ldots$$S_{N,N}$
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

3
101
0??
1??

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

101
010
101

</div>

<p>
It is possible to replace `?`with digits so that the scores of all paths are $3$.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4
2026
?2?8
????
?214

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

-1

</div>

<p>
No replacement can satisfy the condition.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

2
99
99

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

99
99

</div>

</section>

</div>

</span>

</span>

</div>
