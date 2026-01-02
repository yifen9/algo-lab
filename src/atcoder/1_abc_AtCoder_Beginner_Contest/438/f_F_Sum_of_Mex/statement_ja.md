
<div>

<span>

<span>

<p>
配点 : $525$点
</p>

<div>

<section>

### **問題文**

<p>
$N$頂点の木 $T$が与えられます。各頂点には $0$から $N-1$までの番号がついており、 $i$番目 $(1\le i\le N-1)$の辺は頂点 $u_i$と頂点 $v_i$を双方向に繋いでいます。（頂点番号は 0-indexed で辺番号が 1-indexed であることに注意してください。）
</p>

<p>
$0$以上 $N$未満の整数の組 $(i,j)$に対し $f(i,j)$を以下のように定めます：
</p>

<ul>

<li>
木 $T$の頂点 $i$から頂点 $j$までのパスに 
<strong>
含まれない
</strong>
頂点のうち番号が最も小さい頂点の頂点番号。
<ul>

<li>
ただし、頂点 $i$から頂点 $j$までのパスに頂点 $0$から頂点 $N-1$まで全ての頂点が含まれる場合 $f(i,j)=N$とする。
</li>

</ul>

</li>

</ul>

<p>
木 $T$の頂点 $i$から頂点 $j$までのパスに頂点 $i,j$も含まれることに注意してください。
</p>

<p>
$\displaystyle \sum_{0\le i \le j < N} f(i,j)$の値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\le N\le 2\times 10^5$
</li>

<li>
$0\le u_i < v_i < N$
</li>

<li>
入力で与えられるグラフは木
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

$N$$u_1$$v_1$$u_2$$v_2$$\vdots$$u_{N-1}$$v_{N-1}$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$\displaystyle \sum_{0\le i \le j < N} f(i,j)$の値を出力せよ。
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
0 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

3

</div>

<p>
$f(0,0)=1,f(0,1)=2,f(1,1)=0$です。したがって、 $1+2+0=3$を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5
0 1
0 2
2 3
2 4

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

16

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

7
1 4
2 6
0 5
0 3
2 5
1 5

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

16

</div>

</section>

</div>

</span>

</span>

</div>
