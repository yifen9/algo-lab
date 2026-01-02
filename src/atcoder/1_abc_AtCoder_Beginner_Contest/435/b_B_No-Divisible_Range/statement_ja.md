
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
長さ $N$の正整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます。

$1\leq l\leq r\leq N$をみたす整数の組 $(l,r)$であって、
次の条件をみたすものの個数を求めてください。
</p>

<blockquote>

<p>
$l\leq i\leq r$をみたす任意の整数 $i$について、$A_i$は $A_l+A_{l+1}+\cdots+A_r$の約数
<strong>
でない
</strong>
。
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 50$
</li>

<li>
$1 \leq A_i \leq 1000$
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

5
8 6 10 5 7

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

6

</div>

<p>
$A=(8,6,10,5,7)$です。
</p>

<p>
例えば、$(l,r)=(1,2)$は、$A_l+A_{l+1}+\cdots+A_r=A_1+A_2=14$であり、$A_1=8$, $A_2=6$はどちらも $14$の約数でないため、条件をみたします。

一方で、$(l,r)=(1,3)$は、$A_l+A_{l+1}+\cdots+A_r=A_1+A_2+A_3=24$であり、$A_1=8$が $24$の約数であるため、条件をみたしません。
</p>

<p>
条件をみたす組は $(l,r)=(1,2), (1,4), (2,3), (2,4), (3,5), (4,5)$の $6$つであるため、$6$を出力します。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3
1 1 1

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

</span>

</span>

</div>
