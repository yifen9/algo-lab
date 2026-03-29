
<div>

<span>

<span>

<p>
配点 : $900$点
</p>

<div>

<section>

### **問題文**

<p>
正整数 $N, K$が与えられます．
</p>

<p>
左側に $N$個の頂点 $l_1, l_2, …, l_N$，右側に $N$個の頂点 $r_1, r_2, …, r_N$を持つ完全二部グラフ $G$があります．辺の本数は $N^2$であり，各 $(i, j)\ (1\leq i\leq N, 1\leq j\leq N)$に対して頂点 $l_i$と頂点 $r_j$の間に無向辺が $1$つあります．
</p>

<p>
$G$の各辺に $1$以上 $N^2$以下の整数を書き込む（ただし，書き込む $N^2$個の整数は相異なるようにする）方法であって，以下の問題の答えが $K$になるようなものが存在するかどうか判定し，存在するならば書き込み方を一つ求めてください．
</p>

<blockquote>

<p>
グラフ $G$上のウォークのうち，通過した辺に書かれた数を通過順に並べた列が狭義単調増加となるものを良いウォークと呼びます．
</p>

<p>
良いウォークに含まれる辺の本数の最大値を求めてください．
</p>

</blockquote>

<p>
$T$個のテストケースが与えられるので，それぞれについて答えを求めてください．
</p>

<details>

<summary>
ウォークとは
</summary>
グラフ $G$上のウォークとは， $k$個（$k$は正整数）の頂点と $k−1$個の辺を交互に並べた列 $(v_1 ​ ,e_1 ​ ,v_2 ​ ,\ldots,v_{k−1} ​ ,e_{k−1} ​ ,v_k)$であって，辺 $e_i$​が頂点 $v_i$​と頂点 $v_{i+1}$​を結んでいるようなものを指します．

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq T\leq 3000$
</li>

<li>
$1\leq N\leq 700$
</li>

<li>
$1\leq K\leq N^2$
</li>

<li>
一つの入力に含まれる $N^2$の総和は $5\times 10^5$以下
</li>

<li>
入力される数値は全て整数
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

$N$$K$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$\mathrm{case}_1,\mathrm{case}_2,\ldots,\mathrm{case}_T$に対する答えを順に以下の形式で出力せよ．
</p>

<p>
条件を満たす書き込み方が存在しない場合，`No`と出力せよ．
</p>

<p>
存在する場合，頂点 $l_i$と頂点 $r_j$を結ぶ辺に書き込む整数を $A_{i,j}$として，
</p>

<div>

Yes
$A_{1,1}$$A_{1,2}$$\ldots$$A_{1,N}$$A_{2,1}$$A_{2,2}$$\ldots$$A_{2,N}$$\vdots$$A_{N,1}$$A_{N,2}$$\ldots$$A_{N,N}$
</div>

<p>
と出力せよ．$(A_{1,1},\ldots,A_{1,N},A_{2,1},\ldots,A_{2,N},\ldots,A_{N,1},\ldots,A_{N,N})$は $(1,2,\ldots,N^2)$の順列である必要がある．
</p>

<p>
解が複数存在する場合，どれを出力しても正解とみなされる．
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
2 1
2 3
3 5

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

No
Yes
1 2
3 4
Yes
2 9 7
4 5 6
1 8 3

</div>

<p>
$1$つ目のテストケースについて，条件を満たす書き込み方は存在しません．
</p>

<p>
$2$つ目のテストケースについて，辺を $3$本含む良いウォークとして $r_1 \xrightarrow{1} l_1 \xrightarrow{2}r_2\xrightarrow{4}l_2$が存在します．辺を $4$本以上含む良いウォークは存在しないため，この出力は条件を満たします．
</p>

<p>
$3$つ目のテストケースについて，辺を $5$本含む良いウォークとして $l_1 \xrightarrow{2} r_1 \xrightarrow{4}l_2\xrightarrow{6}r_3 \xrightarrow{7} l_1 \xrightarrow{9} r_2$が存在します．辺を $6$本以上含む良いウォークは存在しないため，この出力は条件を満たします．
</p>

<p>

<img src="https://img.atcoder.jp/agc077/483f3ac7fef3640067cde0b569f0be80.png">

</img>

</p>

</section>

</div>

</span>

</span>

</div>
