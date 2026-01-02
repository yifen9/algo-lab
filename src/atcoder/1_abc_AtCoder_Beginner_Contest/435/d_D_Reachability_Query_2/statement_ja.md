
<div>

<span>

<span>

<p>
配点 : $425$点
</p>

<div>

<section>

### **問題文**

<p>
$N$頂点 $M$辺の有向グラフが与えられます。

頂点には $1$から $N$の番号がついており、$i$番目の辺は頂点 $X_i$から頂点 $Y_i$への有向辺です。

最初全ての頂点は白色です。
</p>

<p>
$Q$個のクエリが与えられるので順に処理してください。クエリは以下の $2$種類のいずれかです。
</p>

<ul>

<li>
`1 v`：頂点 $v$を黒色にする
</li>

<li>
`2 v`：頂点 $v$から辺を辿って黒色の頂点に到達可能かどうか判定する
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N \leq 3\times 10^5$
</li>

<li>
$0\leq M \leq 3\times 10^5$
</li>

<li>
$1\leq Q \leq 3\times 10^5$
</li>

<li>
$1\leq X_i,Y_i \leq N$
</li>

<li>
自己辺をもたない。すなわち $X_i \neq Y_i$
</li>

<li>
多重辺をもたない。すなわち $(X_i,Y_i)$は相異なる
</li>

<li>
クエリにおいて $1 \leq v \leq N$
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

$N$$M$$X_1$$Y_1$$\vdots$$X_M$$Y_M$$Q$$\mathrm{query}_1$$\vdots$$\mathrm{query}_Q$
</div>

<p>
$\mathrm{query}_i$は $i$番目のクエリを表し、以下のいずれかの形式で与えられる。
</p>

<div>

$1$$v$
</div>

<div>

$2$$v$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$2$種類目のクエリの個数を $q$として $q$行出力せよ。
</p>

<p>
$i$行目には、$i$番目の $2$種類目のクエリにおいて到達可能なら `Yes`、到達不可能なら `No`と出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

5 6
1 2
2 3
3 1
4 5
1 4
2 5
5
1 3
2 1
2 4
1 5
2 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes
No
Yes

</div>

<ul>

<li>
最初、与えられたグラフは下図一番左の通りです。
</li>

<li>
$1$番目のクエリにより頂点 $3$が黒色になり、下図中央のようになります。
</li>

<li>
$2$番目のクエリにおいて、頂点 $1$から黒色の頂点 $3$に到達可能です。
</li>

<li>
$3$番目のクエリにおいて、頂点 $4$から黒色の頂点に到達することはできません。
</li>

<li>
$4$番目のクエリにより頂点 $5$が黒色になり、下図右のようになります。
</li>

<li>
$5$番目のクエリにおいて、頂点 $4$から黒色の頂点 $5$に到達可能です。
</li>

</ul>

<p>

<img src="https://img.atcoder.jp/abc435/82e480fb4420fdfd7a0f13168774c1fb.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
