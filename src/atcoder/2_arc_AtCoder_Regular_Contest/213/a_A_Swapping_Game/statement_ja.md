
<div>

<span>

<span>

<p>
配点 : $600$点
</p>

<div>

<section>

### **問題文**

<p>
$(1,2, \dots ,L)$の順列が $N$個あります。$i$$(1 \le i \le N)$個目の順列は $P_i$であり、$P_i$の $j$$(1 \le j \le L)$番目の要素は $P_{i,j}$です。
</p>

<p>
はじめ、あなたは $A = (1,2, \dots ,L)$を持っており、所持金は $0$円です。これから、$i = 1,2, \dots ,N$の順に以下の操作を行います。
</p>

<ol>

<li>
まず、$A$の隣接 $2$項の swap を $0$回または $1$回行う。
<ul>

<li>
「$A$の隣接 $2$項の swap」とは、$1 \le j \le L-1$なる $j$を選び、$A_j$と $A_{j+1}$を入れ替える操作を指します。
</li>

</ul>

</li>

<li>
その後、$A = P_i$となっていれば $C_i$円を獲得する。
</li>

</ol>

<p>
最終的なあなたの所持金としてありえる金額の最大値を求めて下さい。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 3 \times 10^4$
</li>

<li>
$1 \leq L \leq 9$
</li>

<li>
$0 \leq C_i \leq 10^4$
</li>

<li>
$P_i$は $(1,2, \dots, L)$の順列
</li>

<li>
入力はすべて整数
</li>

</ul>

</section>

</div>

---

<div>

<div>

<section>

### **入力**

<p>
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$N$$L$$C_1$$P_{1,1}$$P_{1,2}$$\dots$$P_{1,L}$$C_2$$P_{2,1}$$P_{2,2}$$\dots$$P_{2,L}$$\vdots$$C_N$$P_{N,1}$$P_{N,2}$$\dots$$P_{N,L}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 3
200 2 1 3
400 3 1 2
300 2 3 1
100 3 2 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

600

</div>

<p>
以下のように操作を行うことで所持金を $600$円にすることが出来ます。
</p>

<ul>

<li>
$i=1$: $A_1,A_2$を swap し、$A=(2,1,3)$とする。$A=P_1$であるため、$200$円を獲得する。
</li>

<li>
$i=2$: $A_2,A_3$を swap し、$A=(2,3,1)$とする。$A=P_2$でない。
</li>

<li>
$i=3$: swap を行わず、$A=(2,3,1)$のままとする。$A=P_3$であるため、$300$円を獲得する。
</li>

<li>
$i=4$: $A_1,A_2$を swap し、$A=(3,2,1)$とする。$A=P_4$であるため、$100$円を獲得する。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

2 1
0 1
10000 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

10000

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1 9
2025 2 4 6 8 7 5 1 9 3

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

10 5
2615 5 1 3 4 2
4275 1 3 2 5 4
4331 3 1 5 2 4
1457 3 5 1 2 4
2222 1 3 2 4 5
5051 2 4 5 3 1
1082 2 3 1 5 4
1579 4 1 5 2 3
2855 5 1 3 2 4
5848 2 4 3 1 5

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

12345

</div>

</section>

</div>

</span>

</span>

</div>
