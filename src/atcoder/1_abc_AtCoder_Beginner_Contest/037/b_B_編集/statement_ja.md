
<div>

<div>

<div>

<section>

### **問題文**

<p>
長さ $N$の数列 $\{a_i\}$があります。最初、この数列の全ての要素は $0$です。
</p>

<p>
この数列に対し、計 $Q$回次の操作を入力で与えられた順に行ってください。
</p>

<ul>

<li>
数列の $L_i$番目から $R_i$番目 (両端を含む) を $T_i$に書き換える。ただし、数列の最初の要素が $1$番目である。
</li>

</ul>

<p>
最終的に数列の各値が何になったかを求めてください。
</p>

</section>

</div>

---

<div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 100$
</li>

<li>
$1 \leq Q \leq 100$
</li>

<li>
$1 \leq L_i \leq R_i \leq N$
</li>

<li>
$1 \leq T_i \leq 10^9$
</li>

<li>
$T_i$は整数である。
</li>

</ul>

</section>

</div>

<div>

<section>

### **入力**

<p>
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$N$$Q$$L_1$$R_1$$T_1$:
$L_Q$$R_Q$$T_Q$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
出力は $N$行からなる。上から $i$行目に操作後の $a_i$の値を出力せよ。
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
1 3 10
2 4 20

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

10
20
20
20
0

</div>

<p>
最初、数列は $\{0, 0, 0, 0, 0\}$です。
$1$回目の操作の後、数列は $\{10, 10, 10, 0, 0\}$となります。
$2$回目の操作の後、数列は $\{10, 20, 20, 20, 0\}$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

10 4
2 7 22
3 5 4
6 10 1
4 4 12

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0
22
4
12
4
1
1
1
1
1

</div>

</section>

</div>

</div>

</div>
