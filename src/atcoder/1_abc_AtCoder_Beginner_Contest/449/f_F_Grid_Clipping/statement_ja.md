
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
$H$行 $W$列のグリッドがあります。上から $r$行目、左から $c$列目のマスをマス $(r,c)$と呼びます。各マスは黒か白で塗られており、$k=1,2,\ldots,N$に対しマス $(R_k,C_k)$は黒で、それ以外の $HW-N$マスは白で塗られています。
</p>

<p>
このグリッドの中の縦 $h$行、横 $w$列の長方形領域であって、含まれるマスが全て白で塗られているようなものがいくつあるか求めてください。
</p>

<p>
より厳密には、以下の条件を全て満たす整数の組 $(r_0, c_0)$の個数を求めてください。
</p>

<ul>

<li>
$1\le r_0 \le H-h+1$
</li>

<li>
$1\le c_0 \le W-w+1$
</li>

<li>
$0\le i< h,\ 0\le j< w$を満たす全ての整数の組 $(i,j)$に対し、マス $(r_0+i,c_0+j)$は白で塗られている。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le h\le H\le 10^9$
</li>

<li>
$1\le w\le W\le 10^9$
</li>

<li>
$0\le N\le 2\times 10^5$
</li>

<li>
$1\le R_k\le H$
</li>

<li>
$1\le C_k\le W$
</li>

<li>
$(R_{k_1},C_{k_1}) \neq (R_{k_2},C_{k_2})$$(k_1 \neq k_2)$
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

$H$$W$$h$$w$$N$$R_1$$C_1$$R_2$$C_2$$\vdots$$R_N$$C_N$
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

3 4 2 2 3
1 3
2 4
3 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2

</div>

<p>
下図の赤で囲まれた $2$つの長方形領域が条件を全て満たします。
</p>

<p>

<img src="https://img.atcoder.jp/abc449/00912b2ecb8490709ccb3201f77e52a8.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 4 3 2 2
2 2
3 4

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

<p>
条件を全て満たす長方形領域は存在しません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

449 449 3 14 0

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

194892

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

31 9 5 7 10
14 8
8 4
18 8
12 1
8 5
9 6
18 1
14 7
5 6
26 7

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
