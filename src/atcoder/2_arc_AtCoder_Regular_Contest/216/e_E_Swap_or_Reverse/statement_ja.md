
<div>

<span>

<span>

<p>
配点 : $1000$点
</p>

<div>

<section>

### **問題文**

<p>
$(1,2,\ldots,N)$の順列 $P=(P_1,P_2,\ldots,P_N)$および整数の組の集合 $S=\lbrace (x_1, y_1), (x_2,y_2),\ldots,(x_M,y_M)\rbrace$が与えられます．
</p>

<p>
あなたは以下の $2$種類の操作を好きな順番で何度でも行うことができます．
</p>

<ul>

<li>
$(P_l,P_r)\in S$または $(P_r,P_l)\in S$であるような $(l,r)\ (1\leq l\lt r\leq N)$を選び，$P$の $l$番目の要素と $r$番目の要素を入れ替える．すなわち，$P$を $(P_1,\ldots,P_{l-1},P_r,P_{l+1},\ldots,P_{r-1},P_l,P_{r+1},\ldots,P_N)$で置き換える．
</li>

<li>
$(P_l,P_r)\in S$または $(P_r,P_l)\in S$であるような $(l,r)\ (1\leq l\lt r\leq N)$を選び，$P$の $l$番目から $r$番目までの要素を反転する．すなわち，$P$を $(P_1,\ldots,P_{l-1},P_r,P_{r-1},\ldots,P_{l+1},P_l,P_{r+1},\ldots,P_N)$で置き換える．
</li>

</ul>

<p>
操作によって得られる順列のうち，辞書順最小のものを求めてください．
</p>

<p>
$T$個のテストケースが与えられるので，それぞれについて答えを求めてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq T\leq 3\times 10^4$
</li>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq M\leq 2\times 10^5$
</li>

<li>
$P$は $(1,2,\ldots,N)$の順列
</li>

<li>
$1\leq x_i\lt y_i\leq N$
</li>

<li>
$i\neq j$ならば $(x_i,y_i)\neq (x_j,y_j)$
</li>

<li>
全てのテストケースに対する $N$の総和は $2\times 10^5$以下
</li>

<li>
全てのテストケースに対する $M$の総和は $2\times 10^5$以下
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
入力は以下の形式で標準入力から与えられる．
</p>

<div>

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる．
</p>

<div>

$N$$M$$P_1$$P_2$$\ldots$$P_N$$x_1$$y_1$$x_2$$y_2$$\vdots$$x_M$$y_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ．$i$行目には $\mathrm{case}_i$に対する答えを出力せよ．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

2
6 2
1 3 2 5 4 6
1 4
2 5
8 5
7 3 2 8 6 5 1 4
1 8
2 5
3 4
7 8
5 6

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

1 2 5 3 4 6
1 2 3 7 5 6 8 4

</div>

<p>
$1$つ目のテストケースについて，以下のように操作をすることで $P=(1,2,5,3,4,6)$とすることができます．
</p>

<ul>

<li>
はじめ $P=(1,3,2,5,4,6)$である．
</li>

<li>
$(l,r)=(1,5)\ ((P_l,P_r)=(1,4)\in S)$として $1$番目から $5$番目までの要素を反転する．$P=(4,5,2,3,1,6)$となる．
</li>

<li>
$(l,r)=(2,3)\ ((P_r,P_l)=(2,5)\in S)$として $2$番目の要素と $3$番目の要素を入れ替える．$P=(4,2,5,3,1,6)$となる．
</li>

<li>
$(l,r)=(1,5)\ ((P_r,P_l)=(1,4)\in S)$として $1$番目の要素と $5$番目の要素を入れ替える．$P=(1,2,5,3,4,6)$となる．
</li>

</ul>

<p>
これが操作によって得られる辞書順最小の順列です．
</p>

</section>

</div>

</span>

</span>

</div>
