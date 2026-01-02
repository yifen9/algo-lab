
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
$1$から $N$の番号がついた $N$個のマスがあります。最初、どのマスも色が塗られていません。
</p>

<p>
$M$種類の色があり、$i$番目の色ではマス $L_i,L_i+1,\ldots,R_i$のうち好きなマスを好きな個数塗ることができます。
</p>

<p>
以下の条件を満たす色の塗り方は何通りあるか、$998244353$で割った余りを求めてください。
</p>

<ul>

<li>
どのマス $i$についても、そのマスに色が塗られているならば、マス $i-1,i+1$のうちちょうど一方がマス $i$と同じ色で塗られている。
<ul>

<li>
ただし、マス $0,N+1$はどの色にも塗られていないとみなす。
</li>

</ul>

</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N,M \leq 5\times 10^5$
</li>

<li>
$1\leq L_i \leq R_i \leq N$
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

$N$$M$$L_1$$R_1$$\vdots$$L_M$$R_M$
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

5 2
1 3
1 5

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

11

</div>

<p>
$1$番目の色ではマス $1,2,3$を、$2$番目の色ではマス $1,2,3,4,5$を塗ることができます。
</p>

<p>
条件を満たす塗り方は以下の $11$通りです。
</p>

<p>

<img src="https://img.atcoder.jp/abc435/03fd1b0a01e7b5e51ebb60b7b4f1a610.png">

</img>

</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 3
1 1
2 2
3 3

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1

</div>

<p>
どのマスにも色を塗らない $1$通りが条件を満たします。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

500000 10
1 499999
2 499998
3 499997
4 499996
5 499995
6 499994
7 499993
8 499992
9 499991
10 499990

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

775503999

</div>

<p>
$998244353$で割った余りを求めてください。
</p>

</section>

</div>

</span>

</span>

</div>
