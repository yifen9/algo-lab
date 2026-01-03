
<div>

<span>

<span>

<p>
配点 : $425$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $A=(A_1,A_2,\dots,A_N)$が与えられます。

以下を全て満たす整数の $3$つ組 $(i,j,k)$がいくつあるか求めてください。
</p>

<ul>

<li>
$1 \le i,j,k \le N$
</li>

<li>
$A_i : A_j : A_k = 7:5:3$
</li>

<li>
$\min(i,j,k) = j$または $\max(i,j,k) = j$
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
入力は全て整数
</li>

<li>
$1 \le N \le 3 \times 10^5$
</li>

<li>
$1 \le A_i \le 10^9$
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

$N$$A_1$$A_2$$\dots$$A_N$
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

10
3 10 7 10 7 6 7 6 5 14

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

7

</div>

<p>
条件を満たす整数の $3$つ組 $(i,j,k)$は以下の $7$個です。
</p>

<ul>

<li>
$(3,9,1)$
<ul>

<li>
$A_i : A_j : A_k = 7:5:3$であり、 $\max(i,j,k) = j$です。
</li>

</ul>

</li>

<li>
$(5,9,1)$
<ul>

<li>
$A_i : A_j : A_k = 7:5:3$であり、 $\max(i,j,k) = j$です。
</li>

</ul>

</li>

<li>
$(7,9,1)$
<ul>

<li>
$A_i : A_j : A_k = 7:5:3$であり、 $\max(i,j,k) = j$です。
</li>

</ul>

</li>

<li>
$(10,2,6)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$であり、 $\min(i,j,k) = j$です。
</li>

</ul>

</li>

<li>
$(10,2,8)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$であり、 $\min(i,j,k) = j$です。
</li>

</ul>

</li>

<li>
$(10,4,6)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$であり、 $\min(i,j,k) = j$です。
</li>

</ul>

</li>

<li>
$(10,4,8)$
<ul>

<li>
$A_i : A_j : A_k = 14:10:6 = 7:5:3$であり、 $\min(i,j,k) = j$です。
</li>

</ul>

</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

6
210 210 210 210 210 210

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

21
49 30 50 21 35 15 21 70 35 9 50 70 21 49 30 50 70 15 9 21 30

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

34

</div>

</section>

</div>

</span>

</span>

</div>
