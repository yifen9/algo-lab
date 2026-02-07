
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
2 次元座標平面に、 点 $(\frac{A}{C}, \frac{B}{C})$を中心とする半径 $\frac{\sqrt{N}}{C}$の円があります。
この円の円周上にある格子点の個数を $998244353$で割ったあまりを求めてください。
</p>

<p>
なお、 $N$は $N=\prod_{i=1}^{M} P_i^{E_i}$と素因数分解された形で与えられます。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$N \geq 1$
</li>

<li>
$2 \leq P_i \leq 100$
</li>

<li>
$P_i$は相異なる素数
</li>

<li>
$1 \leq E_i \leq 10^{18}$
</li>

<li>
$1 \leq C \leq 50$
</li>

<li>
$0 \leq A,B \lt C$
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

$A$$B$$C$$M$$P_1$$E_1$$P_2$$E_2$$\vdots$$P_M$$E_M$
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

1 1 2 2
2 1
5 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

12

</div>

<p>
下図に示す通り、円周上に $12$個の格子点があります。
</p>

<p>

<img src="https://img.atcoder.jp/abc444/f34d3c88f51a7a212173794f9b2546da.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1 5 14 4
2 1
5 1
13 1
17 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

4

</div>

<p>
下図に示すとおり、円周上に $4$個の格子点があります。
</p>

<p>

<img src="https://img.atcoder.jp/abc444/88d8c0112cd1be716f7355fbaddc93ad.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1 1 6 3
2 1
5 2
13 1

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

6

</div>

<p>
下図に示すとおり、円周上に $6$個の格子点があります。
</p>

<p>

<img src="https://img.atcoder.jp/abc444/fd322921f436a778b10d591f0aebcbe2.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

0 0 1 10
97 1000000000000000000
89 1000000000000000000
73 1000000000000000000
61 1000000000000000000
59 1000000000000000000
47 1000000000000000000
31 1000000000000000000
23 1000000000000000000
11 1000000000000000000
5 1000000000000000000

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

7885876

</div>

<p>
$998244353$で割った余りを求めてください。
</p>

</section>

</div>

</span>

</span>

</div>
