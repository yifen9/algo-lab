
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
$1, 2, 3, 4$の $4$頂点からなる完全グラフがあります。
</p>

<p>
あなたはこれから $6$つの各辺に重みを割り当てます。いずれの重みも正整数であり、$6$つの重みの和がちょうど $K$になるように割り当てます。

より形式的には、$\sum_{1\leq i<j\leq 4}x_{i,j}=K$となる正整数 $x_{i,j} \ (1\leq i<j\leq 4)$を選び、$i, j$を結ぶ辺に重み $x_{i,j}$を割り当てます。
</p>

<p>
この辺に重みをつけたグラフ $G$の 
<strong>
全ての頂点を通る
</strong>
サイクルにおける辺の重みの総和の最小値を $f(G)$とします。
考えうる全ての $G$に対する $f(G)$の総和を $998244353$で割ったあまりを求めて下さい。
</p>

<details>

<summary>
完全グラフとは
</summary>

<p>
任意の異なる $2$頂点間に辺があるグラフを完全グラフと言います。

</p>

</details>

<p>

</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$6 \le K \le 5000$
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

$K$
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

7

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

24

</div>

<p>
$6$つの辺のうち $1$つの重みが $2$であり、それ以外の辺の重みが $1$であるようなグラフが考えられます。
そのようなグラフ $G$は $6$通りあり、いずれの場合も $f(G)=4$であるため、答えは $24$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

2026

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

513760748

</div>

</section>

</div>

</span>

</span>

</div>
