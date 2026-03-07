
<div>

<span>

<span>

<p>
配点 : $100$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $A=(A_1,A_2,\dots,A_N)$と整数 $X$が与えられます。

$i=1,2,\dots,N$の順に以下を行ってください。 
</p>

<ul>

<li>
もし $A_i<X$なら、 $X=A_i$に更新した上で `1`を出力する。
</li>

<li>
そうでないなら `0`を出力する。
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
$1 \le N,X,A_i \le 100$
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

$N$$X$$A_1$$A_2$$\dots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$N$行出力せよ。

そのうち $k$行目には、 $i=k$についての出力をせよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

5 10
6 4 7 1 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

1
1
0
1
0

</div>

<ul>

<li>
最初、 $X=10$です。
</li>

<li>
$i=1$について、 $A_1=6<X=10$なので、 $X=6$に更新した上で `1`を出力します。
</li>

<li>
$i=2$について、 $A_2=4<X=6$なので、 $X=4$に更新した上で `1`を出力します。
</li>

<li>
$i=3$について、 $A_3=7 \ge X=4$なので、 `0`を出力します。
</li>

<li>
$i=4$について、 $A_4=1<X=4$なので、 $X=1$に更新した上で `1`を出力します。
</li>

<li>
$i=5$について、 $A_5=3 \ge X=1$なので、 `0`を出力します。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1 1
1

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

8 20
9 19 14 17 17 4 18 4

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

1
0
0
0
0
1
0
0

</div>

</section>

</div>

</span>

</span>

</div>
