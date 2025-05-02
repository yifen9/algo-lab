
<div>

<span>

<span>

<p>
配点 : $600$点
</p>

<div>

<section>

### **問題文**

<p>
$1$から $N$までの整数からなる順列 $P=(P_1,P_2,\dots,P_N)$と整数 $K$が与えられます。
</p>

<p>
順列 $P$に対して以下のような操作を考えます。
</p>

<ul>

<li>
$1 \leq i \leq N-K+1$を満たす整数 $i$を $1$つ選び、 $P_i,P_{i+1},\dots,P_{i+K-1}$を昇順に並び替える。すなわち、$P_i,P_{i+1},\dots,P_{i+K-1}$を小さい方から順に並べたものを $(x_1,x_2,\dots,x_K)$としたとき、各 $1 \leq j \leq K$に対して $P_{i+j-1}$を $x_j$で置き換える。
</li>

</ul>

<p>
$P$に対して上記の操作をちょうど $1$回行うことで得られる順列のうち、辞書式順序最大のものを求めてください。
</p>

<details>

<summary>
数列の辞書順とは？
</summary>

<p>
数列 $S = (S_1,S_2,\ldots,S_{|S|})$が数列 $T = (T_1,T_2,\ldots,T_{|T|})$より
<strong>
辞書順で小さい
</strong>
とは、下記の 1. と 2. のどちらかが成り立つことを言います。
ここで、$|S|, |T|$はそれぞれ $S, T$の長さを表します。
</p>

<ol>

<li>
$|S| \lt |T|$かつ $(S_1,S_2,\ldots,S_{|S|}) = (T_1,T_2,\ldots,T_{|S|})$。 
</li>

<li>
ある整数 $1 \leq i \leq \min\lbrace |S|, |T| \rbrace$が存在して、下記の $2$つがともに成り立つ。

<ul>

<li>
$(S_1,S_2,\ldots,S_{i-1}) = (T_1,T_2,\ldots,T_{i-1})$
</li>

<li>
$S_i$が $T_i$より（数として）小さい。
</li>

</ul>

</li>

</ol>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq K \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq P_i \leq N$
</li>

<li>
$(P_1,P_2,\dots,P_N)$は $1$から $N$までの整数からなる順列
</li>

<li>
入力される値はすべて整数
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
入力は以下の形式で標準入力から与えられます。
</p>

<div>

$N$$K$$P_1$$P_2$$\dots$$P_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$P$に対して操作をちょうど $1$回行うことで得られる順列のうち、辞書式順序で最大のものを空白区切りで出力してください。
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
2 1 4 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2 1 3 4

</div>

<p>
$i=1$として操作を行うと $(P_1,P_2,P_3)=(2,1,4)$であり、これを昇順に並び替えると $(1,2,4)$となります。よって操作によって $P_1,P_2,P_3$はそれぞれ $1,2,4$に置き換えられ、 $P=(1,2,4,3)$となります。同様に $i=2$として操作を行うと $P$は $(2,1,3,4)$となります。
</p>

<p>
これらのうち辞書式順序で大きいのは $(2,1,3,4)$であるため、答えは $(2,1,3,4)$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 1
3 1 4 2 5

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

3 1 4 2 5

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

20 7
9 4 3 1 11 12 13 15 17 7 2 5 6 20 19 18 8 16 14 10

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

9 4 3 1 11 12 13 15 17 7 2 5 6 8 18 19 20 16 14 10

</div>

</section>

</div>

</span>

</span>

</div>
