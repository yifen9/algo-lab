
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
英小文字からなる $N$個の奇数長の文字列 $S_1,S_2,\dots,S_N$が与えられます。
</p>

<p>
$S_1,S_2,\dots,S_N$のうち最も長いものの長さを $m$とします。
以下の条件を満たす文字列 $T_1,T_2,\dots,T_N$を求めてください。
</p>

<ul>

<li>
条件：$T_i$はある非負整数 $k$について $k$個の `.`、$S_i$、$k$個の `.`をこの順に結合してできる、長さ $m$の文字列である。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$N$は $1$以上 $100$以下の整数
</li>

<li>
$S_i$は英小文字からなる長さ $1$以上 $99$以下の奇数長の文字列
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

$N$$S_1$$S_2$$\vdots$$S_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$N$行出力せよ。$i\ (1 \leq i \leq N)$行目には $T_i$を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4
apple
blueberry
coconut
dragonfruit

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

...apple...
.blueberry.
..coconut..
dragonfruit

</div>

<p>
$m=11$であり、$T_1,T_2,T_3,T_4$はそれぞれ $k=3,1,2,0$について問題文中の条件を満たしています。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

6
abc
d
efghi
jkl
mnopq
r

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

.abc.
..d..
efghi
.jkl.
mnopq
..r..

</div>

</section>

</div>

</span>

</span>

</div>
