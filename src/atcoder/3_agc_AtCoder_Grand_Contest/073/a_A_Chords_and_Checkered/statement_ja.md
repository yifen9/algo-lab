
<div>

<span>

<span>

<p>
配点 : $700$点
</p>

<div>

<section>

### **問題文**

<p>
整数 $L,K$及び長さ $N$の非負整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます．
ここで，$2K < L$及び $0 \leq A_1 < A_2 < \cdots < A_N < L$が保証されます．
</p>

<p>
周の長さが $L$の円を考えます．
この円の適当な点を基準点としてとり，そこから円周上を距離 $x$だけ時計回りに進んだ場所を座標 $x$の点と呼ぶことにします．
また，各 $i$($1 \leq i \leq N$) について， 座標 $A_i$の点と座標 $A_i+K$の点を結ぶ弦を考え，これを弦 $i$と呼ぶことにします．
</p>

<p>
弦の集合 $s$に対して，以下の手順で 
<strong>
スコア
</strong>
を定めます．
</p>

<ul>

<li>
$s$に含まれる弦をすべて描く．描いた弦によって円がいくつかの領域に分かれるので，それらを白と黒で塗る．
まず円の中心が含まれる領域を白く塗り，残りの領域は，(長さ正の線分で)隣接する領域の色が異なるように塗る．
このような塗り方は常に一意に存在することが証明できる．
ここで黒く塗られた領域の個数をスコアとする．
</li>

</ul>

<p>
$s$としてあり得る集合は $2^N$通りあります．
これらすべてに対するスコアの総和を $998244353$で割ったあまりを求めてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq K$
</li>

<li>
$2K < L \leq 10^9$
</li>

<li>
$1 \leq N \leq 250000$
</li>

<li>
$0 \leq A_1 < A_2 < \cdots < A_N < L$
</li>

<li>
入力はすべて整数
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

$L$$K$$N$$A_1$$A_2$$\ldots$$A_N$
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

5 2 2
0 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

4

</div>

<ul>

<li>
弦を $1$つも選ばない場合，スコアは $0$です．
</li>

<li>
弦 $1$を選ぶ場合，スコアは $1$です．
</li>

<li>
弦 $2$を選ぶ場合，スコアは $1$です．
</li>

<li>
弦 $1,2$を選ぶ場合，スコアは $2$です．
</li>

</ul>

<p>
よって，これらの合計である $4$が答えです．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 1 1
2

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

5 2 5
0 1 2 3 4

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

80

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

7 3 3
0 2 3

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

12

</div>

</section>

</div>

</span>

</span>

</div>
