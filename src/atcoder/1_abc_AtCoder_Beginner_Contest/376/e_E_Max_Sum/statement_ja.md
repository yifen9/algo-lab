
<div>

<span>

<span>

<p>
配点 : $475$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の数列 $A = (A_1, A_2, \dots, A_N), B = (B_1, B_2, \dots, B_N)$が与えられます。

$\lbrace 1, 2, \dots, N \rbrace$の部分集合であって大きさが $K$のものを $1$つ選び $S$とします。この時、以下の式の値としてあり得る最小値を求めてください。
</p>

<div>
$\displaystyle \left(\max_{i \in S} A_i\right) \times \left(\sum_{i \in S} B_i\right)$
</div>

<p>
$T$個のテストケースが与えられるので、それぞれに対して答えを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq T \leq 2 \times 10^5$
</li>

<li>
$1 \leq K \leq N \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i, B_i \leq 10^6$
</li>

<li>
全てのテストケースに対する $N$の総和は $2 \times 10^5$以下
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
入力は以下の形式で標準入力から与えられる。ここで $\mathrm{case}_i$は $i$番目のテストケースを意味する。
</p>

<div>

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$N$$K$$A_1$$A_2$$\dots$$A_N$$B_1$$B_2$$\dots$$B_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。$i$行目には $i$番目のテストケースの答えを出力せよ。  
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
3 2
3 7 6
9 2 4
5 3
6 4 1 5 9
8 6 5 1 7
10 6
61 95 61 57 69 49 46 47 14 43
39 79 48 92 90 76 30 16 30 94

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

42
60
14579

</div>

<p>
$1$番目のテストケースでは、$S = \lbrace 2, 3 \rbrace$を選ぶと式の値が $7 \times (2 + 4) = 42$になり、これが最小です。
</p>

</section>

</div>

</span>

</span>

</div>
