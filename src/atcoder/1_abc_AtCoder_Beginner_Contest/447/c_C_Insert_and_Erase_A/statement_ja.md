
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
英大文字からなる文字列 $S,T$が与えられます。
</p>

<p>
あなたは以下の $2$種類の操作を好きな順序で好きな回数（$0$回でも良い）行うことができます。
</p>

<ul>

<li>
$S$の好きな位置（先頭および末尾を含む）に文字 `A`を $1$つ挿入する。
</li>

<li>
$S$に含まれる文字 `A`を $1$つ選んで削除する。なお、残った文字は元の順序を保ったまま連結される。
</li>

</ul>

<p>
$S$を $T$に一致させることが可能かどうか判定し、可能な場合は必要な操作回数の合計の最小値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$S,T$は英大文字からなる長さ $1$以上 $3\times 10^5$以下の文字列
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

$S$$T$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$S$を $T$に一致させることが可能ならば必要な操作回数の合計の最小値を、不可能ならば `-1`を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

ABC
BACA

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
以下のように、合計 $3$回の操作で $S$を $T$に一致させることが可能です。
</p>

<ul>

<li>
$S$の $2$文字目と $3$文字目の間に `A`を $1$つ挿入する。$S=$`ABAC`となる。
</li>

<li>
$S$の $1$文字目にある `A`を削除する。$S=$`BAC`となる。
</li>

<li>
$S$の末尾に `A`を $1$つ挿入する。$S=$`BACA`となる。
</li>

</ul>

<p>
合計 $2$回以下の操作で $S$を $T$に一致させることはできないため、答えは $3$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

ABC
ARC

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

-1

</div>

<p>
どのように操作を行っても、$S$を $T$に一致させることはできません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

ABC
ABC

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

0

</div>

<p>
$1$回も操作を行う必要がありません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

AAAWAZAAAABAAAU
AWAAZABAAAAAUA

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

9

</div>

</section>

</div>

</span>

</span>

</div>
