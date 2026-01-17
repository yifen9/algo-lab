
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
AtCoder 国の公用語は、高橋語と青木語の $2$つの言語です。
</p>

<p>
高橋語と青木語は、どちらもその言語に含まれる単語を表記するのに英小文字の一部を使います。
高橋語では長さ $N$の文字列 $S$に含まれる文字のみを使い、青木語では長さ $M$の文字列 $T$に含まれる文字のみを使います。
</p>

<p>
AtCoder 国の公用語に含まれる $Q$個の単語 $w _ 1,w _ 2,\ldots,w _ Q$が与えられます。
それぞれの単語について、その単語に含まれる文字からその単語が次のうちどれに該当するか判定してください。
</p>

<ul>

<li>
高橋語の単語であることが確定する
</li>

<li>
青木語の単語であることが確定する
</li>

<li>
どちらともいえない
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le26$
</li>

<li>
$1\le M\le26$
</li>

<li>
$S$は英小文字からなる長さ $N$の文字列
</li>

<li>
$S$に含まれる文字は先頭からアルファベット順で昇順に並んでいる
</li>

<li>
$S$に含まれる文字はすべて異なる
</li>

<li>
$T$は英小文字からなる長さ $M$の文字列
</li>

<li>
$T$に含まれる文字は先頭からアルファベット順で昇順に並んでいる
</li>

<li>
$T$に含まれる文字はすべて異なる
</li>

<li>
$1\le Q\le100$
</li>

<li>
$w _ i$は英小文字からなる長さ $1$以上 $100$以下の文字列 $(1\le i\le Q)$
</li>

<li>
$w _ i$は高橋語か青木語のどちらかの単語 $(1\le i\le Q)$
</li>

<li>
$N,M,Q$は整数
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

$N$$M$$S$$T$$Q$$w _ 1$$w _ 2$$\vdots$$w _ Q$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$Q$行にわたって出力せよ。
$i$行目には、$w _ i$が高橋語の単語であることが確定するなら `Takahashi`、青木語の単語であることが確定するなら `Aoki`、どちらとも確定しないなら `Unknown`と出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

6 5
ahikst
aikot
5
asahi
okita
kiai
hash
it

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Takahashi
Aoki
Unknown
Takahashi
Unknown

</div>

<p>
例えば、`a`, `s`, `h`, `i`はすべて高橋語で使われる文字で、`h`は青木語で使われる文字ではないので `asahi`は高橋語の単語であることが確定します。
よって、$1$行目には `Takahashi`と出力してください。
</p>

<p>
`i`および `t`はどちらも高橋語でも青木語でも使われる文字なので `it`は高橋語の単語であるとも青木語の単語であるとも確定しません。
よって、$5$行目には `Unknown`と出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

7 6
ahiknst
ahikos
5
kioki
ohiki
tashi
nishi
kashi

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

Aoki
Aoki
Takahashi
Takahashi
Unknown

</div>

<p>
`o`は高橋語で使われる文字ではないので、はじめ $2$つの単語は青木語の単語であることが確定します。
よって、$1$行目と $2$行目には `Aoki`と出力してください。
</p>

<p>
`t`や `n`は青木語で使われる文字ではないので、続く $2$つの単語は高橋語の単語であることが確定します。
よって、$3$行目と $4$行目には `Takahashi`と出力してください。
</p>

<p>
はじめ $4$つの単語については、末尾が `shi`なら高橋語、末尾が `ki`なら青木語という法則がありますが、`k`, `a`, `s`, `h`, `i`はいずれも高橋語と青木語の両方で使われる文字なので `kashi`がどちらの言語の単語であるかを使われている文字から確定させることはできません。
よって、$5$行目には `Unknown`と出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

13 11
defghiqsvwxyz
acejmoqrtwx
15
qhsqzhd
jcareec
wwqxqew
wxqxwex
jxxrtwa
trtqjxe
sqyggse
xxqwxew
xewwxxw
wwqxwex
xqqxqwq
qxxexxe
teqeroc
eeeqqee
vxdevyy

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

Takahashi
Aoki
Unknown
Unknown
Aoki
Aoki
Takahashi
Unknown
Unknown
Unknown
Unknown
Unknown
Aoki
Unknown
Takahashi

</div>

</section>

</div>

</span>

</span>

</div>
