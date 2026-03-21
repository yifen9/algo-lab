
<div>

<span>

<span>

<p>
配点 : $525$点
</p>

<div>

<section>

### **問題文**

<p>
辺と頂点に番号がついた $N$頂点 $N-1+M$辺の有向グラフがあります。

$1 \leq i \leq M$に対し辺 $i$は頂点 $X_i$から頂点 $Y_i$への有向辺であり、$1 \leq i \leq N-1$に対し辺 $M+i$は頂点 $i+1$から頂点 $i$への有向辺です。
</p>

<p>
辺 $1,2,\dots,M$のうちいくつか( $0$個でもよい) の辺を選ぶ方法は $2^M$通りありますが、そのうち選んだ辺を削除したあとのグラフが強連結となるものは何通りありますか。$998244353$で割った余りを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq M \leq 2\times 10^5$
</li>

<li>
$1 \leq X_i < Y_i \leq N$
</li>

<li>
入力は全て整数
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

$N$$M$$X_1$$Y_1$$X_2$$Y_2$$\vdots$$X_M$$Y_M$
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

4 3
1 4
1 3
2 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

5

</div>

<p>
選ぶ辺の番号の集合が $\{\}, \{1\},\{2\},\{3\},\{2,3\}$の $5$通りのいずれかであるとき、グラフは強連結となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

10 11
1 4
1 4
3 9
2 5
3 4
9 10
6 9
4 10
1 3
8 10
4 7

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1297

</div>

<p>
与えられるグラフは多重辺を持つことがあります。
</p>

</section>

</div>

</span>

</span>

</div>
