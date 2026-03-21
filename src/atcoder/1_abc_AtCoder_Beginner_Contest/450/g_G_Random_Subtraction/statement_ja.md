
<div>

<span>

<span>

<p>
配点 : $575$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の非負整数列 $A$が与えられます。

$A$の要素数が $1$になるまで、以下の操作を繰り返し行います。
</p>

<ul>

<li>
$1 \leq i,j \leq |A|$を満たす相異なる $2$整数 $i,j$を一様ランダムに選ぶ。
</li>

<li>
$A_i,A_j$をそれぞれ $a,b$と置く。
</li>

<li>
$A$から $i$番目の要素と $j$番目の要素を削除する。
</li>

<li>
$A$の末尾に $a-b$を追加する。
</li>

</ul>

<p>
最終的な $A$の唯一の要素を $x$とします。
$x^2$の期待値を $\mod 998244353$で求めてください。
</p>

<details>

<summary>
期待値 $\pmod{998244353}$の定義
</summary>

<p>
求める期待値は必ず有理数になることが証明できます。 また、この問題の制約のもとでは、その値を既約分数 $\frac{P}{Q}$で表した時、$Q \neq 0 \pmod{998244353}$となることも証明できます。 よって、$R \times Q \equiv P \pmod{998244353}, 0 \leq R < 998244353$を満たす整数 $R$が一意に定まります。 この $R$を答えてください。


</p>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq A_i \leq 998244352$
</li>

<li>
入力される値は全て整数
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

$N$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを $1$行で出力せよ。
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
4 5 0

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

665496263

</div>

<p>
まず $(i,j)$として $(3,1)$を選ぶと、数列は $(5,-4)$になります。

次に $(i,j)$として $(1,2)$を選ぶと、数列は $(9)$になります。

$x^2$は $\frac{1}{3}$の確率で $81$、 $\frac{2}{3}$の確率で $1$になり、期待値は $\frac{83}{3}$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5
450 2026 3 21 100

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

669406799

</div>

</section>

</div>

</span>

</span>

</div>
