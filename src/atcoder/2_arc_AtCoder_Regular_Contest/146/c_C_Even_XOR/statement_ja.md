
<div>

<span>

<span>

<p>
配点 : $600$点
</p>

<div>

<section>

### **問題文**

<p>
$0$以上 $2^N$未満の非負整数からなる集合 $S$のうち、以下の条件を満たすものの個数を $998244353$で割ったあまりを出力してください。
</p>

<ul>

<li>
$S$の空でない部分集合 $T$は以下のどちらかを満たす。
<ul>

<li>
$T$の要素数が奇数
</li>

<li>
$T$の全要素の $\mathrm{XOR}$が $0$でない
</li>

</ul>

</li>

</ul>

<details>

<summary>
$\mathrm{XOR}$とは
    
</summary>

<p>
非負整数 $A, B$のビット単位 $\mathrm{XOR}$、$A \oplus B$は、以下のように定義されます。
        
</p>

<ul>

<li>
$A \oplus B$を二進表記した際の $2^k$($k \geq 0$) の位の数は、$A, B$を二進表記した際の $2^k$の位の数のうち一方のみが $1$であれば $1$、そうでなければ $0$である。
</li>

</ul>
例えば、$3 \oplus 5 = 6$となります (二進表記すると: $011 \oplus 101 = 110$)。

一般に $k$個の整数 $p_1, p_2, p_3, \dots, p_k$のビット単位 $\mathrm{XOR}$は $(\dots ((p_1 \oplus p_2) \oplus p_3) \oplus \dots \oplus p_k)$と定義され、これは $p_1, p_2, p_3, \dots p_k$の順番によらないことが証明できます。  
    
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
$1 \le N \le 2 \times 10^5$
</li>

<li>
入力は全て整数である。
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

$N$
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

2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

15

</div>

<p>
$\lbrace 0,2,3 \rbrace$や $\lbrace 1 \rbrace$や $\lbrace \rbrace$は条件を満たします。
</p>

<p>
$\lbrace 0,1,2,3 \rbrace$は条件を満たしません。
</p>

<p>
なぜなら、$\lbrace 0,1,2,3 \rbrace$は部分集合 $\lbrace 0,1,2,3 \rbrace$が要素数が偶数であり、全要素の $\mathrm{XOR}$が $0$であるからです。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

146

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

743874490

</div>

</section>

</div>

</span>

</span>

</div>
