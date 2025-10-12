
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
$2^{30}$未満の正整数 $C,X$が与えられます。
</p>

<p>
以下の条件を全て満たす正整数 $n$が存在するか判定し、存在する場合は一つ求めてください。
</p>

<ul>

<li>
$1\le n < 2^{60}$
</li>

<li>
$(n \oplus C) \bmod n=X$
</li>

</ul>

<p>
ただし、 $n \oplus C$は $n$と $C$のビット単位 $\mathrm{XOR}$を表します。
</p>

<p>
$T$個のテストケースが与えられるので、それぞれについて答えを求めてください。
</p>

<details>

<summary>
ビット単位 $\mathrm{XOR}$演算とは
    
</summary>

<p>
非負整数 $X,Y$のビット単位 $\mathrm{XOR}$、$X \oplus Y$は、以下のように定義されます。
        
</p>

<ul>

<li>
$X \oplus Y$を二進表記した際の $2^k$($k \geq 0$) の位の数は、$X,Y$を二進表記した際の $2^k$の位の数のうち一方のみが $1$であれば $1$、そうでなければ $0$である。
</li>

</ul>
例えば、$3 \oplus 5 = 6$となります (二進表記すると: $011 \oplus 101 = 110$)。


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
$1\le T\le 2\times 10^5$
</li>

<li>
$1\le C,X < 2^{30}$
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

$T$$\text{case}_1$$\text{case}_2$$\vdots$$\text{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$C$$X$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
各テストケースに対する答えを順に改行区切りで出力せよ。
</p>

<p>
各テストケースについて、条件を全て満たす $n$が存在しない場合は `-1`を出力せよ。
</p>

<p>
そうでない場合、条件を全て満たす $n$を出力せよ。
</p>

<p>
条件を全て満たす $n$が複数ある場合、どれを出力しても正答となる。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3
10 6
2 3
777 153

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

7
-1
208

</div>

<p>
$1$つ目のテストケースについて考えます。
</p>

<p>
$n=7$は $(n\oplus C) \bmod n = (7 \oplus 10) \bmod 7 = 13\bmod 7 = 6=X$より条件を全て満たすことが分かります。したがって、 $1$行目には $7$を出力すると正答となります。
</p>

<p>
この他にも $n=12,18,19$などを出力しても正答となります。
</p>

</section>

</div>

</span>

</span>

</div>
