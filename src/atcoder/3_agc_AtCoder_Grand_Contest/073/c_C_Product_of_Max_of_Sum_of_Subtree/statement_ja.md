
<div>

<span>

<span>

<p>
配点 : $1400$点
</p>

<div>

<section>

### **問題文**

<p>
$1$から $N$までの番号がついた $N$頂点からなる木があり，$i$番目の辺は頂点 $A_i$と頂点 $B_i$を結んでいます．
</p>

<p>
今からこの木の各頂点に $-(N-1)$以上 $1$以下の実数をランダムに書き込みます．
乱数の分布はすべて独立な一様分布です．
</p>

<p>
その後，木の
<strong>
スコア
</strong>
を次のように定義します．
</p>

<ul>

<li>
各頂点 $i$について，$x_i$を以下のように定義する．
<ul>

<li>
頂点 $i$を含むような連結な部分グラフの頂点に書かれた値の総和の最大値
</li>

</ul>

</li>

<li>
$0 \leq x_i \leq 1$を満たさない $i$が存在する場合，木のスコアは $0$となる．
</li>

<li>
そうでない場合，木のスコアは $\prod_{1 \leq i \leq N} x_i$となる．
</li>

</ul>

<p>
木のスコアの期待値を $\text{mod }{998244353}$で求めてください．
</p>

<details>

<summary>
期待値 $\text{mod }{998244353}$の定義
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
$1 \leq N \leq 5000$
</li>

<li>
$1 \leq A_i,B_i \leq N$
</li>

<li>
入力されるグラフは木である
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
入力は以下の形式で標準入力から与えられる．
</p>

<div>

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_{N-1}$$B_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

499122177

</div>

<p>
スコアの期待値は $1/2$です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

2
1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

873463809

</div>

<p>
スコアの期待値は $1/8$です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

3
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

842653798

</div>

<p>
スコアの期待値は $13/648$です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

5
1 2
2 3
3 4
4 5

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

132050425

</div>

<p>
スコアの期待値は $41/187500$です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 5**

<div>

8
1 2
1 3
1 4
1 5
5 6
5 7
5 8

</div>

</section>

</div>

<div>

<section>

### **出力例 5**

<div>

243711918

</div>

<p>
スコアの期待値は $2477/30064771072$です．
</p>

</section>

</div>

</span>

</span>

</div>
