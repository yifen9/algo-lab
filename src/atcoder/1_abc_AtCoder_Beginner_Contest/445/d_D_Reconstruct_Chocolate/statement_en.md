
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
There are $N$pieces of a chocolate bar placed on a table.
Piece $i\ (1 \leq i \leq N)$is a rectangle of $h_i$blocks tall and $w_i$blocks wide.
</p>

<p>
It is known that these pieces were obtained by the following procedure.
</p>

<ul>

<li>
Start by holding a chocolate bar of $H$blocks tall and $W$blocks wide. Nothing is placed on the table.
</li>

<li>
Repeat the following operation $N-1$times.
<ul>

<li>
Split the piece currently in hand into two pieces. Both pieces after splitting must be rectangles along the block boundaries.
</li>

<li>
Place one of the pieces on the table, and keep the other piece in hand.
</li>

</ul>

</li>

<li>
Finally, place the piece in hand on the table.
</li>

</ul>

<p>
Find one way to arrange the $N$pieces into a rectangle of $H$blocks tall and $W$blocks wide satisfying the following conditions.
</p>

<ul>

<li>
Different pieces do not overlap.
</li>

<li>
Pieces must not be rotated. That is, for $h \neq w$, a piece of $h$blocks tall and $w$blocks wide cannot be placed as a piece of $w$blocks tall and $h$blocks wide.
</li>

</ul>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1 \leq H \leq 10^9$
</li>

<li>
$1 \leq W \leq 10^9$
</li>

<li>
$2 \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq h_i \leq H$
</li>

<li>
$1 \leq w_i \leq W$
</li>

<li>
It is guaranteed that the input was obtained by the procedure described in the problem statement.
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

$H$$W$$N$$h_1$$w_1$$h_2$$w_2$$\vdots$$h_N$$w_N$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
In a valid arrangement, let the top-left block of piece $i\ (1 \leq i \leq N)$be located at the $x_i$-th row from the top and the $y_i$-th column from the left of the whole rectangle. Output in the following format:
</p>

<div>

$x_1$$y_1$$x_2$$y_2$$\vdots$$x_N$$y_N$
</div>

<p>
If there are multiple valid arrangements, any of them will be accepted.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4 6 6
2 2
1 4
3 1
1 2
3 1
4 2

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

2 2
4 1
1 1
1 2
1 4
1 5

</div>

<p>
The arrangement in the sample output is illustrated below.
</p>

<p>

<img src="https://img.atcoder.jp/abc445/01efc02bf8be59a646abe39db4b95df1.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **Sample Input 2**

<div>

100 100 20
72 7
4 74
17 67
20 67
96 3
1 95
5 81
87 3
3 87
16 67
95 8
100 2
92 1
3 98
92 5
87 3
1 98
19 67
11 74
87 1

</div>

</section>

</div>

<div>

<section>

### **Sample Output 2**

<div>

7 89
90 22
62 22
7 22
4 96
99 1
94 15
7 19
4 9
27 22
4 1
1 99
7 14
1 1
7 9
7 16
100 1
43 22
79 22
7 15

</div>

</section>

</div>

</span>

</span>

</div>
