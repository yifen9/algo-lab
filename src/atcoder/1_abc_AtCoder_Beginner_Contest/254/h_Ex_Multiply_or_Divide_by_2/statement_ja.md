
<div>

<span>

<span>

<p>
配点 : $600$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個の非負整数からなる多重集合 $A=\{ a_1,\ldots,a_N \}, B=\{ b_1,\ldots,b_N \}$が与えられます。

あなたは以下の操作を好きな順番で何度でも行えます。  
</p>

<ul>

<li>
$A$に含まれている非負整数を $1$つ選び、$x$とする。 $A$から $x$を $1$つ削除し、代わりに $2x$を $1$つ追加する。
</li>

<li>
$A$に含まれている非負整数を $1$つ選び、$x$とする。 $A$から $x$を $1$つ削除し、代わりに $\left\lfloor \frac{x}{2} \right\rfloor$を $1$つ追加する。($\lfloor x \rfloor$は $x$を超えない最大の整数)
</li>

</ul>

<p>
あなたの目的は $A$と $B$を(多重集合として)一致させることです。

目的を達成することが出来るかどうかを判定し、出来る場合は必要な操作回数の最小値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 10^5$
</li>

<li>
$0 \leq a_1 \leq \ldots \leq a_N \leq 10^9$
</li>

<li>
$0 \leq b_1 \leq \ldots \leq b_N \leq 10^9$
</li>

<li>
入力はすべて整数
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

$N$$a_1$$\ldots$$a_N$$b_1$$\ldots$$b_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
目的を達成出来る場合は必要な操作回数の最小値を出力せよ。出来ない場合は `-1`を出力せよ。
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
3 4 5
2 4 6

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2

</div>

<p>
次のようにして $2$回の操作で目的を達成できます。  
</p>

<ul>

<li>
$x=3$とし、$A$から $x\, (=3)$を $1$つ削除し代わりに $2x\, (=6)$を $1$つ追加する。これによって $A=\{4,5,6\}$となる。
</li>

<li>
$x=5$とし、$A$から $x\, (=5)$を $1$つ削除し代わりに $\left\lfloor \frac{x}{2} \right\rfloor \, (=2)$を $1$つ追加する。これによって $A=\{2,4,6\}$となる。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1
0
1

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

-1

</div>

<p>
$\{ 0 \}$を $\{ 1 \} $にすることは出来ません。
</p>

</section>

</div>

</span>

</span>

</div>
