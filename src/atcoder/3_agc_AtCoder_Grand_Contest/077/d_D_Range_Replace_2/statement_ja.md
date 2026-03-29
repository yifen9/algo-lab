
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
正整数 $N$と素数 $P$が与えられます．
</p>

<p>
すべての要素が $0$である長さ $N$の数列 $A=(A_1,A_2,\ldots,A_N)$があります．
</p>

<p>
あなたは以下の操作を $0$回以上好きな回数繰り返すことができます．
</p>

<ul>

<li>
整数の組 $(l, r)\ (1\leq l\leq r\leq N)$を選ぶ．$A_l,A_{l+1},\ldots,A_r$を全て $\dfrac{r(r-1)}{2}+l$で置き換える．
</li>

</ul>

<p>
操作を繰り返すことで最終的に得られる $A$としてあり得るものの個数を $P$で割った余りを求めてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N\leq 5000$
</li>

<li>
$P$は $10^8\lt P\lt 10^9$を満たす素数
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

$N$$P$
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

1 998244353

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
得られる $A$は $(0),(1)$の $2$通りです．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

2 998244353

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

7

</div>

<p>
得られる $A$は $(0,0),(0,3),(1,0),(1,2),(1,3),(2,2),(2,3)$の $7$通りです．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

3 998244353

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

38

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

4 998244353

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

282

</div>

</section>

</div>

---

<div>

<section>

### **入力例 5**

<div>

77 777777773

</div>

</section>

</div>

<div>

<section>

### **出力例 5**

<div>

112061248

</div>

</section>

</div>

</span>

</span>

</div>
