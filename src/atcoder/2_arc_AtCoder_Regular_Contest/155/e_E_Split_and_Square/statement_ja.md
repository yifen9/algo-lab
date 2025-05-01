
<div>

<span>

<span>

<p>
配点 : $900$点
</p>

<div>

<section>

### **問題文**

<p>
非負整数からなる集合 $X$に対し、$X$に属する $2$つの整数（同じ整数でもよい）のビット単位 $\mathrm{XOR}$として表せるような非負整数からなる集合を $f(X)$と表します。例えば $X=\lbrace 1, 2, 4\rbrace$に対し $f(X)$は $\lbrace 0, 3, 5, 6\rbrace$となります。
</p>

<p>
$N$個の $2^M$未満の非負整数からなる集合 $S=\lbrace A_1, A_2, \dots, A_N\rbrace$が与えられます。
</p>

<p>
あなたは以下の操作を好きな回数行えます。
</p>

<ul>

<li>
$S$を $2$つの集合 $T_1, T_2$に分ける（ $T_1, T_2$のいずれかが空集合になってもよい）。その後、 $S$を $f(T_1), f(T_2)$の和集合で置き換える。
</li>

</ul>

<p>
$S$を $\lbrace 0\rbrace$にするのに必要な最小の操作回数を求めてください。
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
例えば、$3 \oplus 5 = 6$となります (二進表記すると: $011 \oplus 101 = 110$)。

一般に $k$個の非負整数 $p_1, p_2, p_3, \dots, p_k$のビット単位 $\mathrm{XOR}$は $(\dots ((p_1 \oplus p_2) \oplus p_3) \oplus \dots \oplus p_k)$と定義され、これは $p_1, p_2, p_3, \dots, p_k$の順番によらないことが証明できます。  
    
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
$1 \leq N \leq 300$
</li>

<li>
$1 \leq M \leq 300$
</li>

<li>
$0 \leq A_i < 2^{M}$
</li>

<li>
$A_i\ (1\leq i \leq N)$は互いに相異なる
</li>

<li>
各 $A_i$は $2$進表記でちょうど $M$桁で与えられる（ $A_i$が $M$桁より少ない場合、 leading zero をつけて与えられる）
</li>

<li>
与えられる入力はすべて整数
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

$N$$M$$A_1$$A_2$$\vdots$$A_N$
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

4 2
00
01
10
11

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2

</div>

<p>
$1$回目の操作では $T_1=\lbrace 0, 1\rbrace, T_2=\lbrace 2, 3\rbrace$と分けると $f(T_1) =\lbrace 0, 1\rbrace, f(T_2) =\lbrace 0, 1\rbrace$なので $S$は $\lbrace 0, 1\rbrace$に置き換わります。
</p>

<p>
$2$回目の操作で $T_1=\lbrace 0\rbrace, T_2=\lbrace 1\rbrace$と分けると $S=\lbrace 0\rbrace$となります。
</p>

<p>
$2$回未満の操作で $S$を $\lbrace 0\rbrace$にすることはできないので答えは $2$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1 8
10011011

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1

</div>

<p>
$1$回目の操作で $T_1=\lbrace 155\rbrace, T_2=\lbrace \rbrace$と分けると $S$は $\lbrace 0\rbrace$になります。操作の際は $T_1, T_2$のいずれかが空集合になっても構いません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1 2
00

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

0

</div>

<p>
はじめから $S=\lbrace 0\rbrace$であり、操作する必要がありません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

20 20
10011011111101101111
10100111100001111100
10100111100110001111
10011011100011011111
11001000001110011010
10100111111011000101
11110100001001110010
10011011100010111001
11110100001000011010
01010011101011010011
11110100010000111100
01010011101101101111
10011011100010110111
01101111101110001110
00111100000101111010
01010011101111010100
10011011100010110100
01010011110010010011
10100111111111000001
10100111111000010101

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

10

</div>

</section>

</div>

</span>

</span>

</div>
