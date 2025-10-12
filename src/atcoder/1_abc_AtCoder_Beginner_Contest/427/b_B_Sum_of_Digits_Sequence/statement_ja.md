
<div>

<span>

<span>

<p>
配点 : $200$点
</p>

<div>

<section>

### **問題文**

<p>
正整数 $x$に対して、$f(x)$を $x$の十進表記における各桁の和として定義します。例えば、$f(123) = 1 + 2 + 3 = 6$です。
</p>

<p>
無限数列 $A = (A_0, A_1, A_2, \ldots)$を以下の式により定義します。
</p>

<ul>

<li>
$A_0 = 1$
</li>

<li>
$i \geq 1$のとき $A_i = \displaystyle\sum_{j = 0}^{i - 1} f(A_j)$
</li>

</ul>

<p>
正整数 $N$が与えられます。$A_N$の値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$N$は $1$以上 $100$以下の整数
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

$N$
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

6

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

23

</div>

<ul>

<li>
$A_0 = 1$
</li>

<li>
$A_1 = f(A_0) = 1$
</li>

<li>
$A_2 = f(A_0) + f(A_1) = 2$
</li>

<li>
$A_3 = f(A_0) + f(A_1) + f(A_2) = 4$
</li>

<li>
$A_4 = f(A_0) + f(A_1) + f(A_2) + f(A_3) = 8$
</li>

<li>
$A_5 = f(A_0) + f(A_1) + f(A_2) + f(A_3) + f(A_4) = 16$
</li>

<li>
$A_6 = f(A_0) + f(A_1) + f(A_2) + f(A_3) + f(A_4) + f(A_5) = 23$
</li>

</ul>

<p>
であるため、$A_6 = 23$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

45

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

427

</div>

</section>

</div>

</span>

</span>

</div>
