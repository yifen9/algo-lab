
<div>

<span>

<span>

<p>
配点 : $200$点
</p>

<div>

<section>

### **問題文**

<p>
$H$行 $W$列からなるグリッドがあります。各マスには整数が $1$つずつ書かれており、これらの整数は相異なります。グリッドの上から $i$行目・左から $j$行目のマスには整数 $A_{i,j}$が書かれています。
</p>

<p>
いま、司会が $N$個の相異なる整数 $B_1, \dots, B_N$を叫びました。
</p>

<p>
それぞれの行に対して、司会の叫んだ整数がその行に何個含まれるかを求めたとき、それらの最大値はいくつになりますか？
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq H \leq 3$
</li>

<li>
$1 \leq W \leq 5$
</li>

<li>
$1 \leq N \leq 90$
</li>

<li>
$1 \leq A_{i,j} \leq 90$
</li>

<li>
$A_{i,j}$は相異なる
</li>

<li>
$1 \leq B_i \leq 90$
</li>

<li>
$B_i$は相異なる
</li>

<li>
入力される値はすべて整数
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

$H$$W$$N$$A_{1,1}$$\cdots$$A_{1,W}$$\vdots$$A_{H,1}$$\cdots$$A_{H,W}$$B_1$$\vdots$$B_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
答えを $1$行に出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 4 5
12 3 5 7
6 10 11 9
1 2 4 8
2
4
9
6
11

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3

</div>

<ul>

<li>
上から $1$行目にある整数のうち、司会の叫んだ整数は $0$個です。
</li>

<li>
上から $2$行目にある整数のうち、司会の叫んだ整数は $6,11,9$の $3$個です。
</li>

<li>
上から $3$行目にある整数のうち、司会の叫んだ整数は $2,4$の $2$個です。
</li>

</ul>

<p>
以上より、$0,3,2$のうちの最大値である $3$が答えです。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3 5 2
81 63 31 16 15
30 3 6 54 24
26 41 48 64 66
44
79

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

3 5 12
78 19 70 58 83
12 30 80 20 27
48 71 8 43 82
82
30
43
8
80
70
20
78
12
71
19
48

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

5

</div>

</section>

</div>

</span>

</span>

</div>
