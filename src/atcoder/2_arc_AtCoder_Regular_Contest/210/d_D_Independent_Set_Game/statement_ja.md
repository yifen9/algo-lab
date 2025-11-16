
<div>

<span>

<span>

<p>
配点 : $800$点
</p>

<div>

<section>

### **問題文**

<p>
頂点に $1$から $N$の番号が付いた $N$頂点 $M$辺の単純無向グラフ $G$が与えられます．$i$番目の辺は頂点 $u_i$と頂点 $v_i$を結んでいます．
</p>

<p>
$G$の頂点にははじめ色が塗られていません．Alice と Bob が $G$を使ってゲームをします．Alice と Bob は $t=1,\ldots,N$の順に次の行動を行います．
</p>

<ul>

<li>
$t$が奇数ならば，Alice がまだ色の塗られていない頂点をひとつ選び，その頂点を黒色で塗る．
</li>

<li>
$t$が偶数ならば，Bob がまだ色の塗られていない頂点をひとつ選び，その頂点を白色で塗る．
</li>

</ul>

<p>
$N$回すべての行動が終わった時点で，黒色で塗られた頂点全体が $G$の独立集合であれば Alice が勝者，そうでなければ Bob が勝者となります．両者が最適に行動した場合の勝者の名前を出力してください．
</p>

<p>
$T$個のテストケースが与えられるので，それぞれについて解いてください．
</p>

<details>

<summary>
独立集合とは
</summary>
単純無向グラフ $G$の頂点からなる集合 $S$が $G$の独立集合であるとは，辺で結ばれた $2$頂点 $u,v$であって $u\in S$かつ $v\in S$となるものが存在しないことをいいます．

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq T\leq 2\times 10^5$
</li>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$0\leq M\leq 2\times 10^5$
</li>

<li>
$1\leq u_i < v_i \leq N$
</li>

<li>
与えられるグラフは単純無向グラフである．
</li>

<li>
すべてのテストケースにわたる $N$の総和は $2\times 10^5$以下．
</li>

<li>
すべてのテストケースにわたる $M$の総和は $2\times 10^5$以下．
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
入力は以下の形式で標準入力から与えられます．
</p>

<div>

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各ケースは以下の形式で与えられます．
</p>

<div>

$N$$M$$u_1$$v_1$$\vdots$$u_M$$v_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力してください．$i$行目には $i$番目のテストケースについて，両者が最適に行動した場合の勝者の名前（`Alice`または `Bob`）を出力してください．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3
3 2
1 2
1 3
4 2
1 2
1 3
4 6
1 2
1 3
1 4
2 3
2 4
3 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Bob
Alice
Bob

</div>

<p>
各テストケースで与えられるグラフを図示すると次のようになります．
</p>

<p>

<img src="https://img.atcoder.jp/arc210/d904a1191b2a90eea4c58343a1def228.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
