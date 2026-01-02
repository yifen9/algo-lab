
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
The sky is represented by a $2000 \times 2000$grid.

When looking up at the sky, the cell at the $r$-th row from the top and $c$-th column from the left is called $(r,c)$.
</p>

<p>
Currently, there are clouds $1,2,\dots,N$floating in this sky.

The cell $(r,c)$is covered by cloud $i$if and only if it satisfies $U_i \le r \le D_i$and $L_i \le c \le R_i$.
</p>

<p>
For $k=1,2,\dots,N$, answer the following question:
</p>

<ul>

<li>
Remove only cloud $k$from the $N$clouds. At this point, there are $N-1$clouds floating in the sky. How many cells are not covered by any cloud?
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le U_i \le D_i \le 2000$
</li>

<li>
$1 \le L_i \le R_i \le 2000$
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

$N$$U_1$$D_1$$L_1$$R_1$$U_2$$D_2$$L_2$$R_2$$\vdots$$U_N$$D_N$$L_N$$R_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $N$lines.

The $i$-th line should contain the answer to the question when $k=i$.
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
2 4 1 4
3 3 3 5
1 3 4 6
4 5 3 5
5 5 4 6

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

3999983
3999976
3999982
3999978
3999977

</div>

<p>
The figure shows the top-left $5 \times 6$region of the sky.
</p>

<p>

<img src="https://img.atcoder.jp/abc434/448096fbf51b964b654d545a0122517c.png">

</img>

</p>

<ul>

<li>
When cloud $1$is removed, the number of cells covered by some cloud is $17$, so the number of cells not covered by any cloud is $3999983$.
</li>

<li>
When cloud $2$is removed, the number of cells covered by some cloud is $24$, so the number of cells not covered by any cloud is $3999976$.
</li>

<li>
When cloud $3$is removed, the number of cells covered by some cloud is $18$, so the number of cells not covered by any cloud is $3999982$.
</li>

<li>
When cloud $4$is removed, the number of cells covered by some cloud is $22$, so the number of cells not covered by any cloud is $3999978$.
</li>

<li>
When cloud $5$is removed, the number of cells covered by some cloud is $23$, so the number of cells not covered by any cloud is $3999977$.
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
