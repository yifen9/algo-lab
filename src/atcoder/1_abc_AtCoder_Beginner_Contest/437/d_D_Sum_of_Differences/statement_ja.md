
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
長さ $N$の正整数列 $A = (A_1, A_2, \dots, A_N)$および長さ $M$の正整数列 $B = (B_1, B_2, \dots, B_M)$が与えられます。
</p>

<p>
$\displaystyle \sum_{i=1}^{N} \sum_{j=1}^{M} |A_i - B_j|$の値を $998244353$で割ったあまりを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N,M \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i, B_j < 998244353$
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

$N$$M$$A_1$$A_2$$\cdots$$A_N$$B_1$$B_2$$\cdots$$B_M$
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

4 2
1 6 9 2
3 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

26

</div>

<p>
答えは $|1-3| + |1-1| + |6-3| + |6-1| + |9-3| + |9-1| + |2-3| + |2-1| = 2+0+3+5+6+8+1+1 = 26$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

8 8
185991676 311812083 311812083 84357963 185991676 185991676 724020528 369175631
455049197 387671868 4361724 724020528 724020528 455049197 455049197 724020528

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

529117255

</div>

</section>

</div>

</span>

</span>

</div>
