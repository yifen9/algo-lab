
<div>

<span>

<span>

<p>
配点 : $475$点
</p>

<div>

<section>

### **問題文**

<p>
$N$頂点 $M$辺からなる単純連結無向グラフ $G$が与えられます。
ここで、$N\geq 2$です。
頂点には $1$から $N$までの、辺には $1$から $M$までの番号がそれぞれ付けられており、辺 $i$は頂点 $U_i$と頂点 $V_i$を結んでいます。
また、各辺には 
<strong>
コスト
</strong>
とよばれる値が定められており、辺 $i$のコストは $2^i$です。
</p>

<p>
あなたは今から、$G$の連結成分の個数がちょうど $2$になるように、$G$の辺のうちいくつかを選んで削除します。
（なお、本問題の制約下でこれは必ず達成可能であることが証明できます。）
</p>

<p>
削除する辺のコストの和としてありうる最小値を $998244353$で割った余りを求めてください。
（$998244353$で割った余りを最小化するのではないことに注意してください。）
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\leq N \leq 2\times 10^5$
</li>

<li>
$N-1\leq M \leq \min\left(\frac{N(N-1)}{2}, 2\times 10^5\right)$
</li>

<li>
$1\leq U_i < V_i \leq N$
</li>

<li>
$i\neq j$ならば $(U_i, V_i) \neq (U_j, V_j)$
</li>

<li>
$G$は連結
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

$N$$M$$U_1$$V_1$$U_2$$V_2$$\vdots$$U_M$$V_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
削除する辺のコストの和としてありうる最小値を $998244353$で割った余りを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

5 7
2 3
1 2
1 5
4 5
2 4
3 5
1 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

22

</div>

<p>

<img src="https://img.atcoder.jp/abc447/9a14605fcbaad3095d74d32d6cae6c55.png">

</img>

</p>

<p>
辺 $1,2,4$の $3$本の辺（上図において点線で示されている辺）を削除すると、$G$の連結成分の個数はちょうど $2$になります。
</p>

<p>
このとき、削除する辺のコストの和は $2^1+2^2+2^4=22$であり、これが最小です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

2 1
1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

2

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

8 16
2 7
5 7
6 8
1 7
4 7
1 3
2 8
5 8
4 8
2 5
3 4
3 8
1 4
1 8
4 6
1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

54

</div>

</section>

</div>

</span>

</span>

</div>
