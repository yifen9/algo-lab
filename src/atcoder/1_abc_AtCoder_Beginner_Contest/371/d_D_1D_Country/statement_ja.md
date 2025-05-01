
<div>

<span>

<span>

<p>
配点 : $350$点
</p>

<div>

<section>

### **問題文**

<p>
数直線上に $N$個の村があります。$i$番目の村は座標 $X_i$にあり、$P_i$人の村人がいます。
</p>

<p>
$Q$個のクエリに答えてください。$i$番目のクエリは以下の形式です。
</p>

<ul>

<li>
整数 $L_i,R_i$が与えられる。座標が $L_i$以上 $R_i$以下の村に住んでいる村人の人数の総数を求めよ。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N,Q\leq 2\times 10^5$
</li>

<li>
$-10^9\leq X_1 < X_2 < \ldots < X_N \leq 10^9$
</li>

<li>
$1\leq P_i\leq 10^9$
</li>

<li>
$-10^9\leq L_i \leq R_i \leq 10^9$
</li>

<li>
入力される数値は全て整数
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

$N$$X_1$$\ldots$$X_N$$P_1$$\ldots$$P_N$$Q$$L_1$$R_1$$\vdots$$L_Q$$R_Q$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$Q$行出力せよ。
</p>

<p>
$i\ (1\leq i \leq Q)$行目には、$i$番目のクエリに対する答えを出力せよ。
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
1 3 5 7
1 2 3 4
4
1 1
2 6
0 10
2 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

1
5
10
0

</div>

<p>
$1$番目のクエリについて考えます。座標が $1$以上 $1$以下の村は、座標 $1$にある村で、村人は $1$人います。よって答えは $1$です。
</p>

<p>
$2$番目のクエリについて考えます。座標が $2$以上 $6$以下の村は、座標 $3$にある村と座標 $5$にある村で、村人はそれぞれ $2$人と $3$人います。よって答えは $2+3=5$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

7
-10 -5 -3 -1 0 1 4
2 5 6 5 2 1 7
8
-7 7
-1 5
-10 -4
-8 10
-5 0
-10 5
-8 7
-8 -3

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

26
15
7
26
18
28
26
11

</div>

</section>

</div>

</span>

</span>

</div>
