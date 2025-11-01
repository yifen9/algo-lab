
<div>

<span>

<span>

<p>
配点 : $300$点
</p>

<div>

<section>

### **問題文**

<blockquote>

<p>
AtCoder 国には「トラック運転手は $A$分以上運転する際には $B$分以上の休憩を取らなければならない」というルールがあります。
</p>

</blockquote>

<p>
`a`, `b`からなる長さ $N$の文字列 $S$と正整数 $A,B$が与えられます。以下の条件を全て満たす整数組 $(l,r)$の個数を求めてください。
</p>

<ul>

<li>
$1\leq l \leq r \leq N$
</li>

<li>
$S$の $l$文字目から $r$文字目までに含まれる `a`の個数が $A$以上
</li>

<li>
$S$の $l$文字目から $r$文字目までに含まれる `b`の個数が $B$未満
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N \leq 3\times 10^5$
</li>

<li>
$1 \leq A,B \leq N$
</li>

<li>
$S$は `a`, `b`のみからなる長さ $N$の文字列
</li>

<li>
与えられる数値は全て整数
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

$N$$A$$B$$S$
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

11 4 2
abbaaabaaba

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3

</div>

<p>
条件を満たす $(l,r)$の組は $(4,8),(4,9),(5,9)$の $3$個です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

13 1 2
bbbbbbbbbbbbb

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

<p>
条件を満たす $(l,r)$の組は存在しません。
</p>

</section>

</div>

</span>

</span>

</div>
