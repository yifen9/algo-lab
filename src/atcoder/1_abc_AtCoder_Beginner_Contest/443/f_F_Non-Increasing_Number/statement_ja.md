
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
以下の条件を満たす正整数 $X$を 
<strong>
良い整数
</strong>
とします。
</p>

<ul>

<li>
$X$を十進法で表記したとき一の位、十の位、$\ldots$が広義単調減少になっている。
<ul>

<li>
より厳密には、$\displaystyle X=\sum_{i=0}^{\infty} d_i10^i$$(0\le d_i < 10)$を満たす唯一の非負整数列 $(d_0,d_1,\ldots)$が広義単調減少列になっている。
</li>

</ul>

</li>

</ul>

<p>
例えば、 $112389$や $1$、$777$は良い整数ですが、 $443$や $404$は良い整数ではありません。
</p>

<p>
正整数 $N$が与えられます。
</p>

<p>
$N$の倍数であるような良い整数が存在するか判定し、存在する場合はその最小値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le 3\times 10^6$
</li>

<li>
入力される値は整数
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
$N$の倍数であるような良い整数が存在しない場合は $-1$を出力せよ。
</p>

<p>
存在する場合は $N$の倍数であるような良い整数の最小値を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

21

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

126

</div>

<p>
$126$は $21$の倍数であり、 $6 \geq 2 \geq 1 \geq 0 \geq \ldots$が成り立つため良い整数です。 $126$未満の $21$の倍数であるような良い整数は存在しないため、 $126$を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

10

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

-1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

3

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

3

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

1089

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

9999999999999999999999

</div>

<p>
答えが $2^{64}$以上になる場合があります。
</p>

</section>

</div>

</span>

</span>

</div>
