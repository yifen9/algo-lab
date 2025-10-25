
<div>

<span>

<span>

<p>
配点 : $300$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます。

$1\leq i<j<k\leq N$をみたす整数の組 $(i,j,k)$であって、
次の条件をみたすものの個数を求めてください。
</p>

<blockquote>

<p>
$A_i,A_j,A_k$の中にちょうど $2$種類の値が含まれる。すなわち、$A_i,A_j,A_k$の中のいずれか $2$つは等しく、残りの $1$つは異なる。
</p>

</blockquote>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$3 \leq N \leq 2\times 10^5$
</li>

<li>
$1 \leq A_i \leq N$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
条件をみたす整数の組の個数を出力せよ。
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
3 2 5 2 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

6

</div>

<p>
例えば、$(i,j,k)=(1,2,4)$は、$A_1=3$, $A_2=2$, $A_4=2$の中に $2,3$のちょうど $2$種類の値が含まれるため、条件をみたします。 

これを含めて、$(i,j,k)=(1,2,4),(1,2,5),(1,4,5),(2,3,4),(2,3,5),(3,4,5)$の $6$組が条件をみたします。

よって、$6$を出力します。
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

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

0

</div>

<p>
条件をみたす組が存在しない可能性もあります。
</p>

</section>

</div>

</span>

</span>

</div>
