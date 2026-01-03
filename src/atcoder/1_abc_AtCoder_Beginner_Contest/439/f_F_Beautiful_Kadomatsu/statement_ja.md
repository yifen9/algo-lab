
<div>

<span>

<span>

<p>
配点 : $525$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $k$の数列 $a=(a_1,a_2,\dots,a_k)$が 
<strong>
門松的
</strong>
であることを、以下のようにして定めます。
</p>

<ul>

<li>
$2 \le i \le k-1$かつ $a_{i-1} < a_i$かつ $a_i > a_{i+1}$を満たす整数 $i$の個数を $x$とする。
</li>

<li>
$2 \le i \le k-1$かつ $a_{i-1} > a_i$かつ $a_i < a_{i+1}$を満たす整数 $i$の個数を $y$とする。
</li>

<li>
$x > y$であるとき、またそのときに限り、数列 $a$を 
<strong>
門松的
</strong>
であると言います。
</li>

</ul>

<p>
$(1,2,\dots,N)$の順列 $P$が与えられます。

$P$の (連続でなくともよい) 部分列であって、門松的であるものの個数を $998244353$で割った余りを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
入力は全て整数
</li>

<li>
$1 \le N \le 3 \times 10^5$
</li>

<li>
$P$は $(1,2,\dots,N)$の順列
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

$N$$P_1$$P_2$$\dots$$P_N$
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

4
1 3 4 2

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
$P$の部分列のうち、門松的であるものは以下の $4$つです。
</p>

<ul>

<li>
$(1,3,4,2)$
</li>

<li>
$(1,3,2)$
</li>

<li>
$(1,4,2)$
</li>

<li>
$(3,4,2)$
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1
1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

20
11 10 18 13 12 16 5 19 7 6 17 4 9 1 14 2 20 15 8 3

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

431610

</div>

<p>
例えば、部分列 $a=(10,13,12,5,7,9,20,3)$は門松的です。
</p>

<ul>

<li>
$i=2,7$に対して $a_{i-1} < a_i$かつ $a_i > a_{i+1}$が成り立つので、 $x=2$です。
</li>

<li>
$i=4$に対して $a_{i-1} > a_i$かつ $a_i < a_{i+1}$が成り立つので、 $y=1$です。
</li>

<li>
$x > y$であるので、部分列 $a$は門松的です。
</li>

</ul>

</section>

</div>

</span>

</span>

</div>
