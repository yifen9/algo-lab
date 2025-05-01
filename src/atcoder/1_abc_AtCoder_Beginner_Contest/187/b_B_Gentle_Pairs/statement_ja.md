
<div>

<span>

<span>

<p>
配点 : $200$点
</p>

<div>

<section>

### **問題文**

<p>
$xy$平面上に $1, 2, \dots, N$の番号が付けられた $N$個の点があります。点 $i$は $(x_i, y_i)$にあり、$N$個の点の $x$座標は互いに異なります。  
</p>

<p>
以下の条件を満たす整数の組 $(i, j)\ (i < j)$の個数を求めてください。
</p>

<ul>

<li>
点 $i$と点 $j$を通る直線の傾きが $-1$以上 $1$以下である。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
入力は全て整数
</li>

<li>
$1 \le N \le 10^3$
</li>

<li>
$|x_i|, |y_i| \le 10^3$
</li>

<li>
$i \neq j$ならば $x_i \neq x_j$
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

$N$$x_1$$y_1$$\vdots$$x_N$$y_N$
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

3
0 0
1 2
2 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2

</div>

<p>
$(0, 0)$と $(1, 2)$を通る直線の傾きは $2$、
$(0, 0)$と $(2, 1)$を通る直線の傾きは $\frac{1}{2}$、
$(1, 2)$と $(2, 1)$を通る直線の傾きは $-1$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1
-691 273

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10
-31 -35
8 -36
22 64
5 73
-14 8
18 -58
-41 -85
1 -88
-21 -85
-11 82

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

11

</div>

</section>

</div>

</span>

</span>

</div>
