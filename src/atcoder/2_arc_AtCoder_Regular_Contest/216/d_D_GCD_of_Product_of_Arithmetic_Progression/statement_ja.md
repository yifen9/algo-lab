
<div>

<span>

<span>

<p>
配点 : $1000$点
</p>

<div>

<section>

### **問題文**

<p>
正整数 $N, B, C, D$が与えられます．
</p>

<p>
非負整数 $k$に対し，整数 $a_k$を初項 $Bk+C$，公差 $D$，項数 $N$の等差数列の全項の積，すなわち $a_k=(Bk+C)(Bk+C+D)(Bk+C+2D)\dots(Bk+C+(N-1)D)$で定義します．
</p>

<p>
$a_0,a_1,a_2,\ldots,a_N$の最大公約数を $998244353$で割った余りを求めてください．
</p>

<p>
$T$個のテストケースが与えられるので，それぞれについて答えてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq T\leq 10^5$
</li>

<li>
$1\leq N,B,C,D\leq 10^6$
</li>

<li>
入力は全て整数
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
入力は以下の形式で標準入力から与えられる．
</p>

<div>

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる．
</p>

<div>

$N$$B$$C$$D$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ．$i$行目には $\mathrm{case}_i$に対する答えを出力せよ．
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
3 1 1 1
4 2 2 6
2026 3 22 216

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

6
128
114347907

</div>

<p>
$1$つ目のテストケースについて，$(a_0, a_1, a_2, a_3) = (1 \times 2 \times 3, 2 \times 3 \times 4, 3 \times 4 \times 5, 4 \times 5 \times 6) = (6, 24, 60, 120)$であり，これらの最大公約数は $6$です．
</p>

</section>

</div>

</span>

</span>

</div>
