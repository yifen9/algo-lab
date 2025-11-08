
<div>

<span>

<span>

<p>
配点 : ${500}$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$および正整数 $D$が与えられます。
</p>

<p>
$A$を並び替えることで得られる整数列 $B=(B_1, B_2, \ldots, B_N)$であって、次の条件を満たすものの個数を $998244353$で割ったあまりを求めてください。
</p>

<ul>

<li>
すべての $i\ (1\leq i\leq N-1)$に対して $B_{i+1}\geq B_i-D$が成り立つ。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq D\leq 10^6$
</li>

<li>
$1\leq A_i\leq 10^6$
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

$N$$D$$A_1$$A_2$$\ldots$$A_N$
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

4 1
5 2 1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3

</div>

<p>
条件を満たす整数列は $(1,2,2,5),(2,1,2,5),(2,2,1,5)$の $3$つです。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 10
20 40 60 80 100

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

15 12345
18270 31252 27543 31406 22271 13402 12279 25697 18349 27615 39360 22790 32581 23990 36154

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

858152905

</div>

</section>

</div>

</span>

</span>

</div>
