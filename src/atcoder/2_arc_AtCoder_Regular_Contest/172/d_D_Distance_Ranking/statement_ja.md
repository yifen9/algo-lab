
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
$N$次元空間上に $N$個の点 $p_1, p_2, \dots, p_N$を以下の条件を満たすように配置してください。
</p>

<blockquote>

<p>

<strong>
条件 1
</strong>
点の座標は $0$以上 $10^8$以下の整数で構成される。
</p>

<p>

<strong>
条件 2
</strong>
入力で指定された $(A_1, B_1), (A_2, B_2), \dots, (A_{N(N-1)/2}, B_{N(N-1)/2})$について、$d(p_{A_1}, p_{B_1}) < d(p_{A_2}, p_{B_2}) < \dots < d(p_{A_{N(N-1)/2}}, p_{B_{N(N-1)/2}})$を満たす。ここで、$d(x, y)$は点 $x, y$のユークリッド距離を示す。
</p>

</blockquote>

<p>
なお、本問題の制約下では答えが存在することが証明できます。また、答えが複数通りある場合でも、そのうち $1$つを出力すればよいです。
</p>

<details>

<summary>
ユークリッド距離とは
</summary>
$n$次元空間上の点 $x, y$のユークリッド距離は、$x$の座標を $(x_1, x_2, \dots, x_n)$、$y$の座標を $(y_1, y_2, \dots, y_n)$として、$\sqrt{(x_1-y_1)^2 + (x_2-y_2)^2 + \dots + (x_n-y_n)^2}$と計算されます。

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$3 \leq N \leq 20$
</li>

<li>
$1 \leq A_i < B_i \leq N \ (1 \leq i \leq \frac{N(N-1)}{2})$
</li>

<li>
$(A_1, B_1), (A_2, B_2), \dots, (A_{N(N-1)/2}, B_{N(N-1)/2})$はすべて異なる
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
入力は以下の形式で標準入力から与えられます。  
</p>

<div>

$N$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_{N(N-1)/2}$$B_{N(N-1)/2}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
点 $p_i$$(1 \leq i \leq N)$の座標を $(p_{i, 1}, p_{i, 2}, \dots, p_{i, N})$とするとき、以下の形式で出力してください。
</p>

<div>

$p_{1, 1}$$p_{1, 2}$$\cdots$$p_{1, N}$$p_{2, 1}$$p_{2, 2}$$\cdots$$p_{2, N}$$\vdots$$p_{N, 1}$$p_{N, 2}$$\cdots$$p_{N, N}$
</div>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4
1 2
1 3
2 4
3 4
1 4
2 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3 2 0 0
9 1 0 0
1 8 0 0
9 8 0 0

</div>

<p>
この出力例では座標の第 $3$、第 $4$の成分がすべて $0$なので、以下の $2$次元の図で表すことができます。
</p>

<p>
$d(p_1, p_2) = \sqrt{37}, d(p_1, p_3) = \sqrt{40}, d(p_2, p_4) = \sqrt{49}, d(p_3, p_4) = \sqrt{64}, d(p_1, p_4) = \sqrt{72}, d(p_2, p_3) = \sqrt{113}$であり、正しい順番になっています。
</p>

<div>

<img src="https://img.atcoder.jp/arc172/2df65ad4071e638a89d365f0aaecf25f.png">

</img>

<p>

</p>

</div>

</section>

</div>

</span>

</span>

</div>
