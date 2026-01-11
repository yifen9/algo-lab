
<div>

<span>

<span>

<p>
配点 : $700$点
</p>

<div>

<section>

### **問題文**

<p>
整数 $N,M,X$が与えられます。
</p>

<p>
以下の一連の操作を行い、長さ $N$の非負整数列 $A$を作ります。
</p>

<ul>

<li>
長さ $2$の整数列 $A=(A_1,A_2)$を自由に決める。
</li>

<li>
その後、$A$に対して以下の操作を $N-2$回行う。
</li>

<ul>

<li>
$k=|A|$とする。$x=A_{k-1}, y=A_k$とする。$A$の末尾に $x+y$または $y-x$を追加する。
</li>

</ul>

</ul>

<p>
また、整数列 $A$が良い数列であるとは、以下を満たすことを言います。
</p>

<ul>

<li>
$0 \le A_i \le M \ (1 \le i \le N)$
</li>

<li>
$A_N=X$
</li>

</ul>

<p>
操作によって得られる全ての良い数列に対する $A_1 \times A_2$の総和を $998244353$で割ったあまりを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$3 \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq X \leq M \leq 2 \times 10^5$
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

$N$$M$$X$
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

3 4 3

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
$(0,3,3),(1,4,3),(2,1,3)$などが考えられます。
</p>

<p>
あり得る数列全ての $A_1 \times A_2$の和は $8$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

150000 160000 140000

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

791841701

</div>

</section>

</div>

</span>

</span>

</div>
