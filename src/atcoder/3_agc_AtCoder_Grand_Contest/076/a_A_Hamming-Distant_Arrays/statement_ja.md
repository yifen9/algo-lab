
<div>

<span>

<span>

<p>
配点 : $700$点
</p>

<div>

<section>

### **問題文**

<p>
整数 $N$が与えられます．
$1$以上 $N$以下の整数からなる長さ $N^2$の整数列 $a,b$に対し，その距離 $d(a,b)$を次のように定義します．
</p>

<ul>

<li>
$d(a,b)=$「$a_i \neq b_i$を満たす $i$($1 \leq i \leq N^2$) の個数」
</li>

</ul>

<p>
今から，$1$以上 $N$以下の整数からなる長さ $N^2$の整数列を $N$個作り，それらを $x_1,x_2,\cdots,x_N$とおきます（順番も区別します）．
以下の条件を満たす $(x_1,x_2,\cdots,x_N)$の個数を $998244353$で割ったあまりを求めてください．
</p>

<ul>

<li>
$1$以上 $N$以下の整数からなる長さ $N^2$の整数列 $y$をどのようにとっても，ある $1 \leq i \leq N$が存在し，$d(x_i,y) \geq N^2-N$を満たす．
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 50$
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
入力は以下の形式で標準入力から与えられる．
</p>

<div>

$N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを出力せよ．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

80

</div>

<p>
例えば，$(x_1,x_2)=((1,1,2,2),(1,2,1,2))$は条件を満たしません．
$y=(1,1,1,2)$とすると，$d(x_1,y)=1,d(x_2,y)=1$となるためです．
</p>

<p>
一方，$(x_1,x_2)=((1,1,1,1),(2,2,2,2))$は条件を満たします．
</p>

<p>
条件を満たす $(x_1,x_2)$は $80$通りあります．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

597965565

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

241191911

</div>

</section>

</div>

</span>

</span>

</div>
