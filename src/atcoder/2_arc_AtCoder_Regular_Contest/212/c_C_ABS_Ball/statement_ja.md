
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
$N$個の白いボールがあります。はじめに各ボールを赤か青どちらかの色で塗ります。
</p>

<p>
これら $N$個の赤か青で塗られたボールを、$M$個の区別できる箱のいずれかに入れます。
</p>

<p>
$i$番目の箱に入っている赤、青のボールの数をそれぞれ $a_i, b_i$とします。
</p>

<p>
全てのボールの入れ方に対する $\prod_{1\leq i \le M}|a_i-b_i|$の総和を
$998244353$で割ったあまりを求めて下さい。
</p>

<p>
ただし、$2$つのボールの入れ方が異なるとは、ある $i$について $a_i,b_i$の少なくとも一方が異なることを言います。
</p>

<p>
特に、
<strong>
ボール同士は区別しない
</strong>
ことに注意してください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \le N,M \le  10^7$
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
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$N$$M$
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

2 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

4

</div>

<p>
箱 $1$にボールを入れる方法は $3$通りあります。

赤と青のボールを $1$個ずつ入れる場合、 $|a_1-b_1|=0$です。

赤と青どちらかを $2$個入れる場合、$|a_1-b_1|=2$です。

よって、求めるべき答えは $0 + 2 + 2 = 4$となります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 7

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

10000000 5000000

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

965172629

</div>

</section>

</div>

</span>

</span>

</div>
