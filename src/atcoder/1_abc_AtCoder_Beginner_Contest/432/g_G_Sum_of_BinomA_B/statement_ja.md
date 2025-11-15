
<div>

<span>

<span>

<p>
配点 : $575$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の正整数列 $A=(A_1,A_2,\dots,A_N)$および長さ $M$の正整数列 $B=(B_1,B_2,\dots,B_M)$が与えられます。
</p>

<p>
$\displaystyle \sum_{i=1}^{N} \sum_{j=1}^{M} \binom{A_i}{B_j}$の値を $998244353$で割った余りを求めてください。
</p>

<p>
ここで、$\displaystyle \binom{x}{y}$は $x$個のものの中から $y$個のものを選ぶ場合の数（二項係数）を表し、特に $x < y$のときは $0$です。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N,M \leq 5\times 10^5$
</li>

<li>
$1\leq A_i,B_j \leq 5\times 10^5$
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

$N$$M$$A_1$$A_2$$\dots$$A_N$$B_1$$B_2$$\dots$$B_M$
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

3 2
2 5 4
1 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

25

</div>

<p>
答えは $\displaystyle \binom{2}{1}+\binom{2}{3}+\binom{5}{1}+\binom{5}{3}+\binom{4}{1}+\binom{4}{3}=2+0+5+10+4+4=25$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 4
2 5 1 5
2 1 2 4

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

65

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

6 8
203497 47202 407775 394325 463982 304784
468417 302156 131932 235902 395728 78537 223857 330739

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

602855848

</div>

</section>

</div>

</span>

</span>

</div>
