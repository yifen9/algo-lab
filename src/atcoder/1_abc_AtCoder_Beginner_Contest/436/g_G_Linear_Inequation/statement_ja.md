
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
長さ $N$の正整数列 $A=(A _ 1,A _ 2,\ldots,A _ N)$および正整数 $M$が与えられます。 
</p>

<p>
次の条件を満たす長さ $N$の非負整数列 $x=(x _ 1,x _ 2,\ldots,x _ N)$がいくつあるか求めてください。
</p>

<ul>

<li>
$\displaystyle\sum _ {i=1} ^ NA _ ix _ i\le M$
</li>

</ul>

<p>
答えは非常に大きくなる場合があるので、答えを $998244353$で割った余りを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le100$
</li>

<li>
$1\le A _ i\le100\ (1\le i\le N)$
</li>

<li>
$1\le M\le10 ^ {18}$
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

$N$$M$$A _ 1$$A _ 2$$\ldots$$A _ N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
条件を満たす非負整数列の個数を $998244353$で割った余りを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 6
5 4 3 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

10

</div>

<p>
条件を満たす $x$は $(0,0,0,0),(0,0,0,1),(0,0,0,2),(0,0,0,3),(0,0,1,0),(0,0,1,1),(0,0,2,0),(0,1,0,0),(0,1,0,1),(1,0,0,0)$の $10$個です。
</p>

<p>
よって、`10`を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

6 89
4 7 5 10 7 6

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

38469

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

1 1000000007
1

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

1755655

</div>

<p>
条件を満たす $x$は $1000000008$個あります。
</p>

<p>
これを $998244353$で割った余りである $1755655$を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 4**

<div>

20 738894495848985641
40 58 13 24 65 11 63 29 98 75 40 77 15 50 83 85 35 46 38 37

</div>

</section>

</div>

<div>

<section>

### **出力例 4**

<div>

31156940

</div>

</section>

</div>

</span>

</span>

</div>
