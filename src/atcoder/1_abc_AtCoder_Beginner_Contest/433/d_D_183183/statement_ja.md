
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
正整数 $x,y$に対して $f(x,y)$を以下のように定義します。
</p>

<ul>

<li>
先頭に余分な $0$を付けない十進表記の $x,y$をそれぞれ文字列として解釈しこの順に連結して得られる文字列を $S$としたときの、 $S$を十進表記の整数として解釈した値。
</li>

</ul>

<p>
例えば $f(12,3) = 123$、$f(100,40)=10040$です。
</p>

<p>
正整数 $N,M$と長さ $N$の正整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます。
</p>

<p>
以下の条件を全て満たす整数の組 $(i,j)$の個数を求めてください。
</p>

<ul>

<li>
$1\le i,j\le N$
</li>

<li>
$f(A_i,A_j)$は $M$の倍数
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le 2\times 10^5$
</li>

<li>
$1\le M\le 10^9$
</li>

<li>
$1\le A_i\le 10^9$
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

$N$$M$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
条件を全て満たす整数の組 $(i,j)$の個数を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

2 11
2 42

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2

</div>

<ul>

<li>
$(i,j)=(1,1)$のとき： $f(A_1,A_1)=22$は $11$の倍数です。
</li>

<li>
$(i,j)=(1,2)$のとき： $f(A_1,A_2)=242$は $11$の倍数です。
</li>

<li>
$(i,j)=(2,1)$のとき： $f(A_2,A_1)=422$は $11$の倍数ではありません。
</li>

<li>
$(i,j)=(2,2)$のとき： $f(A_2,A_2)=4242$は $11$の倍数ではありません。
</li>

</ul>

<p>
以上より、条件を全て満たす整数の組は $(i,j)=(1,1),(1,2)$の $2$つです。したがって、 $2$を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 7
2 8 16 183

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

4

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

5 5
1000000000 1000000000 1000000000 1000000000 1000000000

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

25

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

12 13
80 68 862370 82217 8 56 5 168 672624 6 286057 11864

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

10

</div>

</section>

</div>

</span>

</span>

</div>
