
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
長さ $N$の正整数列 $A$と正整数 $K$が与えられます。

数列 $A$に対して、以下の操作を何回でも行うことができます。
</p>

<ul>

<li>
$1$以上 $N$以下の整数 $i$を一つ選び、$A_i$に $K$を足す。
</li>

</ul>

<p>
$\max(A)-\min(A)$としてあり得る値の最小値を求めてください。
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
$1 \leq K \leq 10^9$
</li>

<li>
$1 \leq A_i \leq 10^9$
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

$N$$K$$A_1$$A_2$$\dots$$A_N$
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

3 10
3 21 9

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

4

</div>

<p>
まず、$i=1$を選ぶと数列は $A=(13,21,9)$になります。

次に、$i=3$を選ぶと数列は $A=(13,21,19)$になります。

次に、$i=1$を選ぶと数列は $A=(23,21,19)$になります。

このとき、$\max(A)-\min(A)=23-19=4$となります。

$\max(A)-\min(A)$を $3$以下にすることはできないので、答えは $4$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 6
4 100 5 10 450

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

2

</div>

</section>

</div>

</span>

</span>

</div>
