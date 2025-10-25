
<div>

<span>

<span>

<p>
配点 : $625$点
</p>

<div>

<section>

### **問題文**

<p>
整数 $N,M,A,B,X,R$が与えられます。
</p>

<p>
$\displaystyle \sum_{k=0}^{N-1} X^{(Ak+B) \bmod M}$を $R$で割ったあまりを求めてください。
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
$1\le T\le 100$
</li>

<li>
$1\le N,M,R\le 10^9$
</li>

<li>
$0\le A,B < M$
</li>

<li>
$1\le X < R$
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
各テストケース $\text{case}_i$は以下の形式で与えられる。
</p>

<div>

$N$$M$$A$$B$$X$$R$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。
</p>

<p>
$i$行目には $i$番目のテストケースについて、$\displaystyle \sum_{k=0}^{N-1} X^{(Ak+B) \bmod M}$を $R$で割ったあまりを出力せよ。
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
4 5 2 1 2 1000000000
777 429 33 58 1 1000000000
20251025 429429 777 1025 575757 998244353

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

15
777
445271630

</div>

<p>
$1$つ目のテストケースについて考えます。
</p>

<ul>

<li>
$k=0$のとき： $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 0+1) \bmod 5}=2^1=2$です。
</li>

<li>
$k=1$のとき： $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 1+1) \bmod 5}=2^3=8$です。
</li>

<li>
$k=2$のとき： $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 2+1) \bmod 5}=2^0=1$です。
</li>

<li>
$k=3$のとき： $\displaystyle X^{(Ak+B) \bmod M}=2^{(2\times 3+1) \bmod 5}=2^2=4$です。
</li>

</ul>

<p>
以上より、求める値は $2+8+1+4$を $1000000000$で割ったあまりである $15$です。したがって、 $1$行目には $15$を出力してください。
</p>

</section>

</div>

</span>

</span>

</div>
