
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
縦 $N$マス横 $M$マスのマス目の各マスに $1$以上 $K$以下の整数をひとつずつ書き込み、列 $A,B$を以下のように定義します。
</p>

<ul>

<li>
$i=1,\dots, N$に対し、$A_i$は $i$行目のマスに書かれた整数の最小値
</li>

<li>
$j=1,\dots, M$に対し、$B_j$は $j$列目のマスに書かれた整数の最大値
</li>

</ul>

<p>
$N,M,K$が与えられるので、列対 $(A,B)$としてありうる相異なるものの個数を $998244353$で割った余りを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N,M,K \leq 2\times 10^5$
</li>

<li>
入力はすべて整数である
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

$N$$M$$K$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
列対 $(A,B)$としてありうる相異なるものの個数を $998244353$で割った余りを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

2 2 2

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
$(A_1,A_2,B_1,B_2)$としてありうるものは、$(1,1,1,1),(1,1,1,2),(1,1,2,1),(1,1,2,2),(1,2,2,2),(2,1,2,2),(2,2,2,2)$の $7$通りです。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

1 1 100

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

100

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

31415 92653 58979

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

469486242

</div>

</section>

</div>

</span>

</span>

</div>
