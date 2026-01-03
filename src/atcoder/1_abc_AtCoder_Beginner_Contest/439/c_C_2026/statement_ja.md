
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
正整数 $n$が次の条件を満たす時、$n$を 
<strong>
良い整数
</strong>
と呼びます。
</p>

<ul>

<li>
$0 \lt x \lt y$かつ $x^2+y^2=n$を満たす整数の組 $(x,y)$がただ $1$つ存在する。
</li>

</ul>

<p>
例えば $n=2026$とすると、$0 \lt x \lt y$かつ $x^2+y^2=n$を満たす整数の組は $(x,y)=(1,45)$しか存在しないことが確認できます。よって $2026$は良い整数です。
</p>

<p>
正整数 $N$が与えられます。$N$以下の良い整数を全て列挙してください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 10^7$
</li>

<li>
$N$は整数
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

$N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$N$以下の良い整数が $k$個あり、それらを昇順に並べた列が $(a_1, a_2, \dots, a_k)$であるとする。この時、以下の形式で答えを出力せよ。($k=0$である場合は $2$行目は空行として出力せよ。)
</p>

<div>

$k$$a_1$$a_2$$\dots$$a_k$
</div>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

10

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2
5 10

</div>

<p>
$0 \lt x \lt y$かつ $x^2+y^2=5$を満たす整数の組は $(x,y)=(1,2)$しか存在しないので $5$は良い整数です。

$0 \lt x \lt y$かつ $x^2+y^2=10$を満たす整数の組は $(x,y)=(1,3)$しか存在しないので $10$は良い整数です。

$N$以下の良い整数はこの $2$個のみです。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1

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

50

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

14
5 10 13 17 20 25 26 29 34 37 40 41 45 50

</div>

</section>

</div>

</span>

</span>

</div>
