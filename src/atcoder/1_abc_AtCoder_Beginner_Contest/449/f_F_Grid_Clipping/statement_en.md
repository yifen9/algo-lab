
<div>

<span>

<span>

<p>
Score : $500$points
</p>

<div>

<section>

### **Problem Statement**

<p>
There is a grid with $H$rows and $W$columns. The cell at the $r$-th row from the top and $c$-th column from the left is called cell $(r,c)$. Each cell is painted black or white: cell $(R_k,C_k)$is black for $k=1,2,\ldots,N$, and the remaining $HW-N$cells are white.
</p>

<p>
Find the number of rectangular regions in this grid with $h$rows and $w$columns such that all cells contained in them are painted white.
</p>

<p>
More formally, find the number of pairs of integers $(r_0, c_0)$satisfying all of the following conditions:
</p>

<ul>

<li>
$1\le r_0 \le H-h+1$
</li>

<li>
$1\le c_0 \le W-w+1$
</li>

<li>
Cell $(r_0+i,c_0+j)$is painted white for all pairs of integers $(i,j)$satisfying $0\le i< h,\ 0\le j< w$.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\le h\le H\le 10^9$
</li>

<li>
$1\le w\le W\le 10^9$
</li>

<li>
$0\le N\le 2\times 10^5$
</li>

<li>
$1\le R_k\le H$
</li>

<li>
$1\le C_k\le W$
</li>

<li>
$(R_{k_1},C_{k_1}) \neq (R_{k_2},C_{k_2})$$(k_1 \neq k_2)$
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

$H$$W$$h$$w$$N$$R_1$$C_1$$R_2$$C_2$$\vdots$$R_N$$C_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output the answer.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

3 4 2 2 3
1 3
2 4
3 1

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
The two rectangular regions enclosed in red in the figure below satisfy all the conditions.
</p>

<p>

<img src="https://img.atcoder.jp/abc449/00912b2ecb8490709ccb3201f77e52a8.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

4 4 3 2 2
2 2
3 4

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

0

</div>

<p>
No rectangular region satisfies all the conditions.
</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 3**

<div>

449 449 3 14 0

</div>

</section>

</div>

<div>

<section>

### **Sample Output 3**

<div>

194892

</div>

</section>

</div>

---

<div>

<section>

### **Sample Input 4**

<div>

31 9 5 7 10
14 8
8 4
18 8
12 1
8 5
9 6
18 1
14 7
5 6
26 7

</div>

</section>

</div>

<div>

<section>

### **Sample Output 4**

<div>

12

</div>

</section>

</div>

</span>

</span>

</div>
