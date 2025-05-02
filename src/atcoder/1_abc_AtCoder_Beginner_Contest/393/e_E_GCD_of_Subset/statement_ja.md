
<div>

<span>

<span>

<p>
配点 : $475$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の数列 $A=(A_1,A_2,\dots,A_N)$と $N$以下の正整数 $K$が与えられます。

$i=1,2,\dots,N$について次の問題を解いてください。
</p>

<ul>

<li>
$A_i$を含むように $K$個の要素を $A$から選ぶ時、それらの最大公約数 (GCD) としてあり得る最大値を求めてください。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq K \leq N \leq 1.2 \times 10^6$
</li>

<li>
$1 \leq A_i \leq 10^6$
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
$N$行出力せよ。$j$行目には $i=j$の時の答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

5 2
3 4 6 7 12

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3
4
6
1
6

</div>

<p>
$i=1$の時は $A_1$と $A_3$を選ぶと最大公約数が $\gcd(\lbrace 3, 6 \rbrace) = 3$となり、これが最大です。

$i=2$の時は $A_2$と $A_5$を選ぶと最大公約数が $\gcd(\lbrace 4, 12 \rbrace) = 4$となり、これが最大です。

$i=3$の時は $A_3$と $A_5$を選ぶと最大公約数が $\gcd(\lbrace 6, 12 \rbrace) = 6$となり、これが最大です。

$i=4$の時は $A_4$と $A_2$を選ぶと最大公約数が $\gcd(\lbrace 7, 4 \rbrace) = 1$となり、これが最大です。

$i=5$の時は $A_5$と $A_3$を選ぶと最大公約数が $\gcd(\lbrace 12, 6 \rbrace) = 6$となり、これが最大です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 3
6 10 15

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1
1
1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10 3
414003 854320 485570 52740 833292 625990 909680 885153 435420 221663

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

59
590
590
879
879
590
20
879
590
59

</div>

</section>

</div>

</span>

</span>

</div>
