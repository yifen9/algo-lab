
<div>

<span>

<span>

<p>
配点 : $450$点
</p>

<div>

<section>

### **問題文**

<p>
`A`, `B`, `C`の $3$種類の文字からなる長さ $N$の文字列 $S$が与えられます。
</p>

<p>
$S$の空でない連続する部分文字列は $\dfrac{N(N+1)}2$個ありますが、そのうち `A`が `B`よりも多く含まれるものはいくつあるか求めてください。
</p>

<p>
$2$つの部分文字列は、$S$から取り出す場所が異なれば文字列として等しくても区別して数えることに注意してください。
</p>

<details>

<summary>
部分文字列とは
</summary>

<p>
$S$の
<strong>
部分文字列
</strong>
とは、$S$の先頭から $0$文字以上、末尾から $0$文字以上削除して得られる文字列のことをいいます。

例えば、`AB`は `ABC`の部分文字列ですが、`AC`は `ABC`の部分文字列ではありません。
</p>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le5\times10 ^ 5$
</li>

<li>
$S$は `A`, `B`, `C`からなる長さ $N$の文字列
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

$N$$S$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$S$の連続する部分文字列のうち `A`が `B`よりも多く含まれるものの個数を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

10
ACBBCABCAB

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

8

</div>

<p>
以下の $8$つの部分文字列が条件を満たします。
</p>

<ul>

<li>
`A`：$S$の $1$文字目から $1$文字目
</li>

<li>
`AC`：$S$の $1$文字目から $2$文字目
</li>

<li>
`CA`：$S$の $5$文字目から $6$文字目
</li>

<li>
`CABCA`：$S$の $5$文字目から $9$文字目
</li>

<li>
`A`：$S$の $6$文字目から $6$文字目
</li>

<li>
`ABCA`：$S$の $6$文字目から $9$文字目
</li>

<li>
`CA`：$S$の $8$文字目から $9$文字目
</li>

<li>
`A`：$S$の $9$文字目から $9$文字目
</li>

</ul>

<p>
これら以外の部分文字列は条件を満たさないため、`8`を出力してください。
</p>

<p>
`A`や `CA`は複数箇所から取り出すことができますが、取り出す場所が異なれば区別して数えることに注意してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4
CCBC

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
条件を満たす部分文字列が存在しないこともあります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

36
CABACBBBBBAABABACCBCABCCABAABABBCBAC

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

136

</div>

</section>

</div>

</span>

</span>

</div>
