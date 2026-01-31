
<div>

<span>

<span>

<p>
配点 : $575$点
</p>

<div>

<section>

### **問題文**

<p>
整数 $N,M,A,B$が与えられます。
</p>

<p>
整数列 $X=(X_0,X_1,\ldots,X_{N-1})$を $\displaystyle X_k = (Ak+B) \bmod M$として定義します。
</p>

<p>
$X_k > k$を満たす $0$以上 $N$未満の整数 $k$の個数を求めてください。
</p>

<p>
$T$個のテストケースが与えられるので、それぞれについて答えを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le T\le 3\times 10^5$
</li>

<li>
$1\le N \le M\le 10^9$
</li>

<li>
$0\le A,B < M$
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

$N$$M$$A$$B$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
各テストケースに対する答えを順に改行区切りで出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4
4 6 4 3
7 7 3 1
10 46 0 12
443 2026 131 210

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2
3
10
395

</div>

<p>
$1$つ目のテストケースについて考えます。
</p>

<ul>

<li>
$k=0$のとき： $X_0=(4\times 0+3)\bmod 6=3$なので、 $X_k>k$が成立します。
</li>

<li>
$k=1$のとき： $X_1=(4\times 1+3)\bmod 6=1$なので、 $X_k>k$は成立しません。
</li>

<li>
$k=2$のとき： $X_2=(4\times 2+3)\bmod 6=5$なので、 $X_k>k$が成立します。
</li>

<li>
$k=3$のとき： $X_3=(4\times 3+3)\bmod 6=3$なので、 $X_k>k$は成立しません。
</li>

</ul>

<p>
以上より、$X_k>k$が成立する $0$以上 $4$未満の整数 $k$は $k=0,2$の $2$個です。したがって、 $1$行目には $2$を出力してください。
</p>

</section>

</div>

</span>

</span>

</div>
