
<div>

<span>

<span>

<p>
配点 : $1200$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の非負整数列 $A=(A_1,A_2,\dots,A_N),B=(B_1,B_2,\dots,B_N)$が与えられます。
</p>

<p>
$(1,2,\dots,N)$の順列 $P=(P_1,P_2,\dots,P_N)$に対して、$P$のコストを $\sum_{i=1}^{N} \left \lfloor \frac{A_{P_i}}{2^{B_i}} \right \rfloor$と定義します。
</p>

<p>
コストの最小値を達成する $P$の個数を $998244353$で割った余りを求めてください。
</p>

<p>
$T$個のテストケースが与えられるので、それぞれについて解いてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \le T \le 2 \times 10^5$
</li>

<li>
$1 \le N \le 2 \times 10^5$
</li>

<li>
$1 \le A_i \le 10^9$
</li>

<li>
$0 \le B_i \le 30$
</li>

<li>
全てのテストケースにおける $N$の総和は $2 \times 10^5$以下
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

$T$$\mathrm{case}_1$$\mathrm{case}_2$$\vdots$$\mathrm{case}_T$
</div>

<p>
各テストケースは以下の形式で与えられる。
</p>

<div>

$N$$A_1\ A_2\ \dots\ A_N$$B_1\ B_2\ \dots\ B_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。$i(1 \le i \le T)$行目には $\mathrm{case}_i$の答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

7
2
5 9
0 1
3
3 4 10
0 1 2
4
1 2 3 4
0 0 1 1
5
1000000000 1000000000 1000000000 1000000000 1000000000
0 0 0 0 0
11
19 68 97 62 99 52 57 19 43 80 96
5 3 3 2 3 4 3 2 3 4 3
14
86 49 83 31 5 43 7 46 98 36 60 4 69 59
3 1 4 4 4 0 1 3 0 4 3 5 1 2
10
907139744 237517128 852012347 350549430 62876062 196019710 263351472 184393437 281593038 753973502
23 12 1 26 29 24 0 7 10 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

1
2
4
120
8640
15552
1

</div>

<p>
$1$個目のテストケースについては、各 $P$に対するコストは以下のようになります。
</p>

<ul>

<li>
$P=(1,2)$のとき、$\left \lfloor \frac{A_{1}}{2^{B_1}} \right \rfloor + \left \lfloor \frac{A_{2}}{2^{B_2}} \right \rfloor = \left \lfloor \frac{5}{1} \right \rfloor + \left \lfloor \frac{9}{2} \right \rfloor = 9$
</li>

<li>
$P=(2,1)$のとき、$\left \lfloor \frac{A_{2}}{2^{B_1}} \right \rfloor + \left \lfloor \frac{A_{1}}{2^{B_2}} \right \rfloor = \left \lfloor \frac{9}{1} \right \rfloor + \left \lfloor \frac{5}{2} \right \rfloor = 11$
</li>

</ul>

<p>
よって、コストの最小値は $9$であり、それを達成する $P$は $(1,2)$の $1$個です。
</p>

<p>
$2$個目のテストケースについては、$P = (1,2,3),(2,1,3)$がコストの最小値 $7$を達成します。
</p>

<p>
$3$個目のテストケースについては、$P = (1,2,3,4),(2,1,3,4),(1,2,4,3),(2,1,4,3)$がコストの最小値 $6$を達成します。
</p>

<p>
$4$個目のテストケースについては、$(1,2,3,4,5)$の順列全てがコストの最小値 $5000000000$を達成します。
</p>

</section>

</div>

</span>

</span>

</div>
