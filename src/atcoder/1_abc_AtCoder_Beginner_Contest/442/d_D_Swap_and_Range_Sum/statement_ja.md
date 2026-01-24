
<div>

<span>

<span>

<p>
配点 : $400$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の数列 $A=(A_1,A_2,\dots,A_N)$が与えられます。
</p>

<p>
$Q$個のクエリが与えられるので、順に処理してください。
各クエリは以下のいずれかの形式です。
</p>

<ul>

<li>
`1 x`: $A_x$と $A_{x+1}$の値を入れ替える。
</li>

<li>
`2 l r`: $\displaystyle \sum_{l\leq i\leq r} A_i$の値を求める。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\leq N \leq 2\times 10^5$
</li>

<li>
$1\leq Q \leq 5\times 10^5$
</li>

<li>
$1\leq A_i \leq 10^4$
</li>

<li>
$1$種類目のクエリについて、$1\leq x \leq N-1$
</li>

<li>
$2$種類目のクエリについて、$1\leq l\leq r \leq N$
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
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$N$$Q$$A_1$$A_2$$\dots$$A_N$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
ここで、$\text{query}_i$は $i$番目のクエリを表し、以下のいずれかの形式で与えられる。
</p>

<div>

$1$$x$
</div>

<div>

$2$$l$$r$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$2$種類目のクエリの個数を $q$として、$q$行出力せよ。
$i$行目 $(1\leq i \leq q)$には、$2$種類目のクエリのうち $i$個目のものに対する答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 4
2 7 1 8
1 2
2 1 2
1 1
2 2 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3
17

</div>

<ul>

<li>
$1$番目のクエリでは、$A_2$と $A_3$の値を入れ替えます。これにより、$A=(2,1,7,8)$になります。
</li>

<li>
$2$番目のクエリでは、$A_1+A_2$の値を求めます。答えは $2+1=3$です。
</li>

<li>
$3$番目のクエリでは、$A_1$と $A_2$の値を入れ替えます。これにより、$A=(1,2,7,8)$になります。
</li>

<li>
$4$番目のクエリでは、$A_2+A_3+A_4$の値を求めます。答えは $2+7+8=17$です。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

8 10
22 75 26 45 72 81 47 29
2 2 7
2 6 8
2 4 4
1 2
2 1 3
1 1
2 2 4
1 2
1 4
2 1 1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

346
157
45
123
142
26

</div>

</section>

</div>

</span>

</span>

</div>
