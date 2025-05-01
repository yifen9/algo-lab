
<div>

<span>

<span>

<p>
配点 : $675$点
</p>

<div>

<section>

### **問題文**

<p>
頂点に $1$から $N$の番号がついた $N$頂点 $M$辺の連結無向グラフが与えられます。グラフは自己ループを含みませんが、多重辺を含む可能性があります。辺には色がついていて、$i$番目の辺は頂点 $u_i$と頂点 $v_i$を結ぶ色 $c_i$($1 \leq c_i \leq C$) の辺です。 また、数列 $A = (A_1, A_2, \dots, A_C)$が与えられます。
</p>

<p>
このグラフの全域木のうち次の条件を満たすものを 
<strong>
カラフル全域木
</strong>
と呼びます。
</p>

<ul>

<li>
$1 \leq i \leq C$を満たす全ての整数 $i$について、全域木に含まれる色 $i$の辺の本数は $A_i$本以下である。
</li>

</ul>

<p>
$1 \leq L \leq R \leq C$を満たす整数の組 $(L, R)$のうち次の条件を満たすものの個数を求めてください。
</p>

<ul>

<li>
カラフル全域木 $T$であって、$T$に含まれる任意の辺の色 $c$が $L \leq c \leq R$を満たすようなものが存在する。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \leq N \leq 150$
</li>

<li>
$N - 1 \leq M \leq \min\left(\frac{CN(N-1)}{2}, 5 \times 10^5\right)$
</li>

<li>
$1 \leq C \leq 300$
</li>

<li>
$1 \leq A_i \leq N-1$
</li>

<li>
$\sum_{i=1}^C A_i \leq 300$
</li>

<li>
$1 \leq u_i \lt v_i \leq N$
</li>

<li>
$1 \leq c_i \leq C$
</li>

<li>
$i \neq j$ならば $(u_i,v_i,c_i) \neq (u_j,v_j,c_j)$
</li>

<li>
入力で与えられるグラフは連結
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

$N$$M$$C$$A_1$$A_2$$\dots$$A_C$$u_1$$v_1$$c_1$$u_2$$v_2$$c_2$$\vdots$$u_M$$v_M$$c_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$1 \leq L \leq R \leq C$を満たす整数の組 $(L, R)$のうち問題文の条件を満たすものの個数を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 4 3
1 2 1
1 2 1
1 2 2
1 3 3
2 3 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

4

</div>

<p>
例えば $(L, R) = (1, 2)$は問題文の条件を満たします。これは $1$番目の辺と $4$番目の辺からなる全域木 $T$はカラフル全域木で、かつ $T$に含まれる任意の辺の色が $L$以上 $R$以下であるからです。

問題文の条件を満たす $(L, R)$は $(1, 2), (1, 3), (2, 2), (2, 3)$の $4$個です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 10 6
2 2 4 1 1 1
1 3 2
1 5 4
2 3 3
1 4 1
4 5 1
4 5 3
2 4 1
1 4 3
1 3 4
1 2 5

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

11

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10 20 5
2 4 4 6 4
5 9 1
4 5 2
2 8 5
8 9 4
1 10 5
8 10 1
8 9 5
4 8 2
4 10 4
5 8 3
5 9 5
6 10 2
3 5 4
4 6 1
3 4 3
7 9 3
5 7 1
1 3 3
1 8 5
5 10 4

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

2

</div>

</section>

</div>

</span>

</span>

</div>
