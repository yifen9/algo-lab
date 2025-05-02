
<div>

<span>

<span>

<p>
配点 : $1400$点
</p>

<div>

<section>

### **問題文**

<p>
非負整数 $X$があり、はじめその値は $S$です。以下の操作を任意の順に何度でも行うことができます。
</p>

<ul>

<li>
$X$に $1$を足す。この操作のコストは $A$である。
</li>

<li>
$1$以上 $N$以下の $i$を選び、$X$を $X \oplus Y_i$に置き換える。この操作のコストは $C_i$である。ここで、$\oplus$はビット単位 $\mathrm{XOR}$演算を表す。
</li>

</ul>

<p>
与えられた非負整数 $T$に $X$を等しくするのに必要な最小の合計コストを求めるか、それが不可能であることを報告してください。
</p>

<details>

<summary>
ビット単位 $\mathrm{XOR}$演算とは
    
</summary>

<p>
非負整数 $A, B$のビット単位 $\mathrm{XOR}$、$A \oplus B$は、以下のように定義されます。
        
</p>

<ul>

<li>
$A \oplus B$を二進表記した際の $2^k$($k \geq 0$) の位の数は、$A, B$を二進表記した際の $2^k$の位の数のうち一方のみが $1$であれば $1$、そうでなければ $0$である。
</li>

</ul>
例えば、$3 \oplus 5 = 6$となります（二進表記すると: $011 \oplus 101 = 110$）。

一般に、$k$個の非負整数 $p_1, p_2, p_3, \dots, p_k$のビット単位 $\mathrm{XOR}$は $(\dots ((p_1 \oplus p_2) \oplus p_3) \oplus \dots \oplus p_k)$と定義され、これは $p_1, p_2, p_3, \dots, p_k$の順番によらないことが証明できます。  
    
<p>

</p>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 8$
</li>

<li>
$0 \leq S, T < 2^{40}$
</li>

<li>
$0 \leq A \leq 10^5$
</li>

<li>
$0 \leq Y_i < 2^{40}$($1 \leq i \leq N$)
</li>

<li>
$0 \leq C_i \leq 10^{16}$($1 \leq i \leq N$)
</li>

<li>
入力中の値は全て整数である。
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
入力は、標準入力から以下の形式で与えられる。
</p>

<div>

$N$$S$$T$$A$$Y_1$$C_1$$\vdots$$Y_N$$C_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
課題が達成不可能なら、`-1`を出力せよ。
そうでないなら、必要な最小の合計コストを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

1 15 0 1
8 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

5

</div>

<p>
以下の方法で $X$を $T$と等しくすることができます。
</p>

<ul>

<li>
$i=1$を選んで $X$を $X \oplus 8$に置き換え、$X=7$とする。この操作のコストは $2$である。
</li>

<li>
$X$に $1$を足し、$X=8$とする。この操作のコストは $1$である。
</li>

<li>
$i=1$を選んで $X$を $X \oplus 8$に置き換え、$X=0$とする。この操作のコストは $2$である。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 21 10 100
30 1
12 1
13 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

3

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1 2 0 1
1 1

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

-1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

8 352217 670575 84912
239445 2866
537211 16
21812 6904
50574 8842
380870 5047
475646 8924
188204 2273
429397 4854

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

563645

</div>

</section>

</div>

</span>

</span>

</div>
