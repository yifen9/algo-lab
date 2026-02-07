
<div>

<span>

<span>

<p>
配点 : $400$点
</p>

<div>

<section>

### **問題文**

<p>
$i=1,2,\dots,N$に対して、$1$を $A_i$個つなげた整数を $B_i$と表します。

より厳密には、$B_i=\sum_{j=0}^{A_i-1}{10^j}$と表します。

$\sum_{i=1}^{N}{B_i}$を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i \leq 2 \times 10^5$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを $1$行で出力せよ。
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
3 3 3 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

444

</div>

<p>
$B_1=B_2=B_3=B_4=111$なので、$B_1+B_2+B_3+B_4=444$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3
30 10 20

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

111111111122222222223333333333

</div>

<p>
答えは非常に大きくなる可能性があります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10
1 2 3 4 5 6 7 8 9 10

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

1234567900

</div>

</section>

</div>

</span>

</span>

</div>
