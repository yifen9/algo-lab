
<div>

<span>

<span>

<p>
配点 : $400$点
</p>

<div>

<section>

### **問題文**

<p>
`A`, `B`, `C`の $3$種類の文字のみからなる文字列 $S$が与えられます。
</p>

<p>
操作を以下のように定義します。
</p>

<blockquote>

<p>
$1 \le i \lt j \lt k \le |S|$かつ $S_i =$`A`, $S_j =$`B`, $S_k =$`C`を満たす $(i, j, k)$の組を選び、$S$の $i, j, k$文字目を取り除く。残った文字を元の順序を保ったまま左に詰める。
</p>

</blockquote>

<p>
文字列 $S$に対して最大で何回操作を行うことができるかを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \le |S| \le 10 ^{6}$
</li>

<li>
$S$は `A`, `B`, `C`のみからなる文字列である
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

$S$
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

ABACBCC

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
以下のように操作をすることで $2$回操作できます。
</p>

<ul>

<li>

<p>
`ABACBCC`に対して $(i, j, k) = (1, 2, 7)$として操作する。残った文字列は `ACBC`となる。
</p>

</li>

<li>

<p>
`ACBC`に対して $(i, j, k) = (1, 3, 4)$として操作する。残った文字列は `C`となる。
</p>

</li>

</ul>

<p>
$3$回以上操作することはできないため、答えは $2$となります。よって $2$と出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

CBACBB

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

BBBAAABCBCBAACBBCAAC

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
