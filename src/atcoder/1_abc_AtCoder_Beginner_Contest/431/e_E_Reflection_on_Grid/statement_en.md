
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
There is a grid with $H$rows and $W$columns. We will refer to the cell at the $i$-th row from the top and $j$-th column from the left as cell $(i,j)$. Each cell has at most one mirror placed on it.
</p>

<p>
Takahashi is standing on the left side of cell $(1,1)$, and Aoki is standing on the right side of cell $(H,W)$. Takahashi has a flashlight and is shining light from the left side of cell $(1,1)$toward the right. Here, assume that the flashlight's light does not diffuse and is a light ray that travels straight.
</p>

<p>
Takahashi's goal is to deliver the flashlight's light to Aoki by using the mirrors in the grid.
</p>

<p>
There are three types of mirror placements. When light hits a mirror, the direction of the light changes according to the mirror placement. For each mirror placement, the exit direction for each entry direction is as shown in the figures below.
</p>

<ul>

<li>
Type A (no mirror is placed)
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc431/9a3821cb76d936b95b6979e084d56994.png">

</img>

</p>

<ul>

<li>
Type B (a mirror is placed on the diagonal connecting the upper-left and lower-right)
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc431/283ea6eabada389e76e89518fcb9fb18.png">

</img>

</p>

<ul>

<li>
Type C (a mirror is placed on the diagonal connecting the upper-right and lower-left)
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc431/9410773fd7615321f27f070d5f0b1844.png">

</img>

</p>

<p>
The mirror placement on the grid is represented by $H$strings of length $W$: $S_1,S_2,\ldots,S_H$. When the $j$-th character of $S_i$is `A`, cell $(i,j)$is type A; when it is `B`, cell $(i,j)$is type B; when it is `C`, cell $(i,j)$is type C.
</p>

<p>
Takahashi can perform the following operation any number of times to deliver the light to Aoki:
</p>

<ul>

<li>
Choose one cell and change the mirror placement of that cell to a different type.
</li>

</ul>

<p>
Find the minimum number of operations needed to deliver the light to Aoki.
</p>

<p>
You are given $T$test cases; find the answer for each.
</p>

</section>

</div>

<div>

<section>

### **Constraints**

<ul>

<li>
$1\leq T$
</li>

<li>
$1\leq H,W$
</li>

<li>
$HW\leq 2\times 10^5$
</li>

<li>
$S_i$is a string of length $W$consisting of `A`, `B`, `C`.
</li>

<li>
$T$, $H$, and $W$are integers.
</li>

<li>
The sum of $HW$over all test cases is at most $2\times 10^5$.
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
Each test case is given in the following format:
</p>

<div>

$H$$W$$S_1$$S_2$$\vdots$$S_H$
</div>

</section>

</div>

<div>

<section>

### **Output**

<p>
Output $T$lines. The $i$-th line should contain the answer for the $i$-th test case.
</p>

</section>

</div>

</div>

---

<div>

<section>

### **Sample Input 1**

<div>

4
3 4
ABCB
CACC
BCBA
2 2
CB
AA
1 10
BCBCBCBCBC
10 10
CCAABACAAA
CCCBACACCA
BACAABCBBA
ACCCAACCCA
CCAAAACCBA
AACBBACCAA
BCCCACBBAB
CBBCAACCCC
CBBCCBCBCA
BBACABBACC

</div>

</section>

</div>

<div>

<section>

### **Sample Output 1**

<div>

0
2
10
5

</div>

<p>
For the first test case, the light can be delivered to Aoki without performing any operations.
</p>

<p>

<img src="https://img.atcoder.jp/abc431/f66a190627b09b9e6c4cbacb84b6d9bd.png">

</img>

</p>

<p>
For the second test case, by changing the mirror placement of cell $(1,1)$to type A and the mirror placement of cell $(2,2)$to type B, the light can be delivered to Aoki as shown in the figure below. It is impossible to deliver the light to Aoki with one or fewer operations, so the answer is $2$.
</p>

<p>

<img src="https://img.atcoder.jp/abc431/1aeac5f2fecf4319d369b8cc3067959a.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
