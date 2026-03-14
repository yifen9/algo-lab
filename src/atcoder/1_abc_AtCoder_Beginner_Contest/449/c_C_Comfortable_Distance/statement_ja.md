
<div>

<span>

<span>

<p>
配点 : $300$点
</p>

<div>

<section>

### **問題文**

<p>
英小文字からなる長さ $N$の文字列 $S$が与えられます。
</p>

<p>
整数の組 $(i, j)$であって、以下の条件をすべて満たすものの個数を求めてください。
</p>

<ul>

<li>
$1 \leq i \leq j \leq N$
</li>

<li>
$S_i = S_j$
</li>

<li>
$L \leq j - i \leq R$
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \leq N \leq 5 \times 10^5$
</li>

<li>
$1 \leq L \leq R \leq N - 1$
</li>

<li>
$N, L, R$は整数
</li>

<li>
$S$は長さ $N$の英小文字からなる文字列
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

$N$$L$$R$$S$
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

6 2 4
aabcba

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
問題文中の条件をすべて満たす整数の組は $(i, j) = (2, 6), (3, 5)$の $2$つです。 
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

9 3 6
aaaaaaaaa

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

18

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10 2 6
aabbccaabb

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

6

</div>

</section>

</div>

</span>

</span>

</div>
