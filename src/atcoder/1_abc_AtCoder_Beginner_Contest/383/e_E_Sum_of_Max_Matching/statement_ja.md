
<div>

<span>

<span>

<p>
配点 : $500$点
</p>

<div>

<section>

### **問題文**

<p>
頂点に $1$から $N$の番号が、辺に $1$から $M$の番号が付いた $N$頂点 $M$辺の重み付き単純連結無向グラフが与えられます。辺 $i$$(1 \leq i \leq M)$は頂点 $u_i$と頂点 $v_i$を双方向に結び、重みは $w_i$です。
</p>

<p>
あるパスに対してその重みをそのパスに含まれる辺の重みの最大値とします。
また、$f(x,y)$を 頂点 $x$から頂点 $y$へのパスの重みとしてありえる最小値とします。
</p>

<p>
長さ $K$の数列　$(A_1,A_2,\ldots,A_K)$と $(B_1,B_2,\ldots,B_K)$が与えられます。ここで、$A_i \neq B_j$$(1 \leq i,j \leq K)$が成り立つことが保証されます。
</p>

<p>
数列 $B$を自由に並べ替えて、$\displaystyle\sum_{i=1}^{K}f(A_i,B_i)$を最小化してください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \leq N  \leq 2 \times 10^5$
</li>

<li>
$N-1 \leq M  \leq \min(\frac{N \times (N-1)}{2},2 \times 10^5)$
</li>

<li>
$1 \leq K \leq N$
</li>

<li>
$1 \leq u_i<v_i \leq N$$(1 \leq i \leq M)$
</li>

<li>
$1 \leq w_i \leq 10^9$
</li>

<li>
$1 \leq A_i,B_i \leq N$$(1 \leq i \leq K)$
</li>

<li>
$A_i \neq B_j$$(1 \leq i,j \leq K)$
</li>

<li>
与えられるグラフは単純かつ連結
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

$N$$M$$K$$u_1$$v_1$$w_1$$u_2$$v_2$$w_2$$\vdots$$u_M$$v_M$$w_M$$A_1$$A_2$$\ldots$$A_K$$B_1$$B_2$$\ldots$$B_K$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$\displaystyle\sum_{i=1}^{K}f(A_i,B_i)$の最小値を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 4 3
1 3 2
3 4 1
2 4 5
1 4 4
1 1 3
4 4 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

8

</div>

<p>
$B$を並び替えて、$B=(2,4,4)$としたとき、
</p>

<ul>

<li>
$f(1,2)=5$: 頂点 $1$から頂点 $4$を経由し頂点 $2$に行くパスがあり、辺 $3$の重み $5$が最大値を取ります。また、辺の重みの最大値が $4$以下になるようなパスは存在しないため $5$が最小値です。
</li>

<li>
$f(1,4)=2$: 頂点 $1$から頂点 $3$を経由し頂点 $4$に行くパスがあり、辺 $1$の重み $2$が最大値を取ります。また、辺の重みの最大値が $1$以下になるようなパスは存在しないため $2$が最小値です。
</li>

<li>
$f(3,4)=1$: 頂点 $3$から頂点 $4$への辺を通るパスがあり、辺の重みは $1$でこれが辺の重みの最大値です。また、パスの重みが $0$以下になることはないため $1$が最小値です。
</li>

</ul>

<p>
よって、この場合 $\displaystyle \sum_{i=1}^{3}f(A_i,B_i)=5+2+1=8$となります。また、$B$をどのように並び替えても $7$以下になることはないため、答えは $8$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 3 2
1 2 5
2 3 2
1 3 1
1 1
2 3

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

3

</div>

</section>

</div>

</span>

</span>

</div>
