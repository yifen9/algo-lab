
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
$0 \leq x,y \leq M-1$を満たす整数組 $(x, y)$のうち、以下の漸化式で表される無限長の数列 $(s_1, s_2, \dots)$が $M$の倍数を全く含まないようなものは何通りありますか？
</p>

<ul>

<li>
$s_1 = x$
</li>

<li>
$s_2 = y$
</li>

<li>
$s_n = A s_{n-1} + B s_{n-2}$($n \geq 3$)
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \leq M \leq 1000$
</li>

<li>
$0 \leq A, B \leq M-1$
</li>

<li>
入力される値はすべて整数
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

$M$$A$$B$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを $1$行に出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

7

</div>

<p>
問題文中の条件を満たす整数組は $(x,y) = (1,1), (1,3), (2,1), (2,2), (2,3), (3,1), (3,3)$の $7$通りです。
</p>

<p>
たとえば $(x,y) = (2,1)$としたとき、対応する数列は $(2,1,5,7,17,31,65,127,\dots)$となります。この数列は $4$の倍数を全く含みません。よって、$(x,y) = (2,1)$は問題文中の条件を満たします。
</p>

<p>
一方で $(x,y) = (3,2)$としたとき、対応する数列は $(3,2,8,12,28,52,108,212,\dots)$となります。この数列の第 $3$項は $8$であり、これは $4$の倍数です。よって、$(x,y) = (3,2)$は問題文中の条件を満たしません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

446 1 1

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
問題文中の条件を満たす整数組は存在しません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1000 784 385

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

995373

</div>

</section>

</div>

</span>

</span>

</div>
