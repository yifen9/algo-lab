
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
英小文字からなる長さ $N$の文字列 $S$が与えられます。
</p>

<p>
長さ $K$の文字列 $t$の
<strong>
出現回数
</strong>
を、以下を満たす整数 $i$の個数として定義します。
</p>

<ul>

<li>
$1 \leq i \leq N-K+1$
</li>

<li>
$S$の $i$文字目から $i+K-1$文字目までからなる部分文字列が $t$に一致する。
</li>

</ul>

<p>
長さ $K$の文字列に対する出現回数の最大値 $x$を求めてください。
また、出現回数が $x$となるような長さ $K$の文字列をすべて辞書順昇順に出力してください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$N, K$は整数
</li>

<li>
$S$は英小文字からなる長さ $N$の文字列
</li>

<li>
$1 \leq K \leq N \leq 100$
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

$N$$K$$S$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$2$行出力せよ。
</p>

<p>
$1$行目には、長さ $K$の文字列に対する出現回数の最大値 $x$を出力せよ。
</p>

<p>
$2$行目には、出現回数が $x$となるような長さ $K$の文字列を辞書順昇順に、空白区切りで出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

9 3
ovowowovo

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2
ovo owo

</div>

<p>
出現回数 $2$の文字列として、以下が挙げられます。
</p>

<ul>

<li>
文字列 `ovo`について、$i=1,7$が条件を満たすことから、`ovo`の出現回数は $2$です。
</li>

<li>
文字列 `owo`について、$i=3,5$が条件を満たすことから、`owo`の出現回数は $2$です。
</li>

</ul>

<p>
出現回数が $2$よりも大きいような長さ $3$の文字列は存在しないので、求める最大値は $2$です。
</p>

<p>
一方で、出現回数が $2$よりも小さい文字列として、以下が挙げられます。
</p>

<ul>

<li>
文字列 `vow`について、$i=2$が条件を満たすことから、`vow`の出現回数は $1$です。
</li>

<li>
文字列 `ooo`について、条件を満たす $i$が存在しないことから、`ooo`の出現回数は $0$です。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

9 1
ovowowovo

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

5
o

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

35 3
thequickbrownfoxjumpsoverthelazydog

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

2
the

</div>

</section>

</div>

</span>

</span>

</div>
