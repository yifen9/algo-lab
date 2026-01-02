
<div>

<span>

<span>

<p>
配点 : $400$点
</p>

<div>

<section>

### **問題文**

<blockquote>

<p>
すぬけ君は蛇を観察しており、どこからどこまでが頭・胴・尾なのかが気になっています。
すぬけ君は蛇を $N$個のブロックに区切り、それぞれのブロックについて頭らしさ・胴らしさ・尾らしさを評価しました。
そして、
<em>
らしさ
</em>
の合計が最大になる分け方を考えることにしました。
</p>

</blockquote>

<p>
長さ $N$の整数列 $A = (A_1, A_2, \ldots, A_N)$, $B = (B_1, B_2, \ldots, B_N)$, $C = (C_1, C_2, \ldots, C_N)$が与えられます。 
</p>

<p>
整数の組 $(x, y)$が $1 \leq x < y < N$を満たすとき、$\displaystyle\sum_{i = 1}^{x} A_i + \sum_{i = x + 1}^{y} B_i + \sum_{i = y + 1}^{N} C_i$の値として取り得る最大値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$3 \leq N \leq 3 \times 10^5$
</li>

<li>
$1 \leq A_i, B_i, C_i \leq 10^6$
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

$N$$A_1$$A_2$$\ldots$$A_N$$B_1$$B_2$$\ldots$$B_N$$C_1$$C_2$$\ldots$$C_N$
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

5
1 4 2 4 3
2 3 4 2 2
3 2 4 4 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

16

</div>

<p>
$(x, y) = (2, 3)$とすると $\displaystyle\sum_{i = 1}^{x} A_i + \sum_{i = x + 1}^{y} B_i + \sum_{i = y + 1}^{N} C_i = 1 + 4 + 4 + 4 + 3 = 16$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3
1 1 1
1 1 1
1 1 1

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

6
2 10 7 7 7 11
5 7 9 10 9 12
6 6 7 10 12 7

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

50

</div>

</section>

</div>

</span>

</span>

</div>
