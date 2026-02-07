
<div>

<span>

<span>

<p>
配点 : $450$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $(A_1,\dots,A_N)$と正整数 $D$が与えられます。
</p>

<p>
以下の条件をともに満たす整数の組 $(L,R)$の個数を求めてください。
</p>

<ul>

<li>
$1 \leq L \leq R \leq N$
</li>

<li>
$(A_L,A_{L+1},\dots,A_R)$のどの $2$つの要素も差が $D$以上である
<ul>

<li>
すなわち、 $L \leq i < j \leq R$を満たす全ての整数の組 $(i,j)$について、 $|A_i-A_j|\geq D$である
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\leq N \leq 4\times 10^5$
</li>

<li>
$1 \leq A_i \leq 10^9$
</li>

<li>
$1 \leq D \leq 10^9$
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

$N$$D$$A_1$$\dots$$A_N$
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

5 3
3 1 4 1 5

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
$(1,1),(2,2),(3,3),(4,4),(5,5),(2,3),(3,4),(4,5)$の $8$組が条件を満たします。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

9 1
1 2 3 4 5 6 7 8 9

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

45

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

6 1000000000
123456789 234567891 987654321 321987654 1000000000 1

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

6

</div>

</section>

</div>

</span>

</span>

</div>
