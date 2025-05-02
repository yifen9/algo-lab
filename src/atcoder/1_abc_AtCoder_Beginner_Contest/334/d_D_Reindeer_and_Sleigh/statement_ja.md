
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
$N$台のソリがあり、各ソリには $1,2,\ldots, N$の番号がつけられています。
</p>

<p>
ソリ $i$を引くために必要なトナカイは $R_i$匹です。
</p>

<p>
また、各トナカイが引けるソリは高々 $1$台です。より厳密には、$m$台のソリ $i_1, i_2, \ldots, i_m$を引くために必要なトナカイは $\sum_{k=1}^{m} R_{i_k}$匹です。
</p>

<p>
以下の形式のクエリが $Q$個与えられるので、答えを求めてください。
</p>

<ul>

<li>
整数 $X$が与えられる。トナカイが $X$匹いるときに最大で何台のソリを引けるか求めよ。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N, Q \leq 2 \times 10^5$
</li>

<li>
$1 \leq R_i \leq 10^9$
</li>

<li>
$1 \leq X \leq 2 \times 10^{14}$
</li>

<li>
入力される数値はすべて整数
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

$N$$Q$$R_1$$R_2$$\ldots$$R_N$$\text{query}_1$$\text{query}_2$$\vdots$$\text{query}_Q$
</div>

<p>
各クエリは次の形式で与えられる。
</p>

<div>

$X$
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
$i$行目には $i$個目のクエリに対する答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 3
5 3 11 8
16
7
1000

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3
1
4

</div>

<p>
トナカイが $16$匹いるとき、ソリ $1,2,4$を引くことができます。
</p>

<p>
$16$匹のトナカイで $4$台のソリを引くことはできないので、クエリ $1$の答えは $3$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

6 6
1 2 3 4 5 6
1
2
3
4
5
6

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1
1
2
2
2
3

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

2 2
1000000000 1000000000
200000000000000
1

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

2
0

</div>

</section>

</div>

</span>

</span>

</div>
