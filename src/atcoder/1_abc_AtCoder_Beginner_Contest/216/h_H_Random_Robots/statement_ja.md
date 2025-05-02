
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
数直線上に $K$個のロボットが置かれています。$i \, (1 \leq i \leq K)$番目のロボットははじめ、座標 $x_i$に存在します。
</p>

<p>
これから以下の操作をちょうど $N$回行います。
</p>

<ul>

<li>
$K$個のロボットそれぞれについて、「進む」か「止まる」かを確率 $\frac{1}{2}$で決める。「進む」と決めたロボットたちは
<strong>
同時に
</strong>
正の方向に $1$進み、「止まる」と決めたロボットたちはその場から動かない。
</li>

</ul>

<p>
ただし、すべての確率的な決定は独立であるとします。
</p>

<p>
一連の操作の中で、複数のロボットが出会う、すなわち $2$個以上のロボットが同時に同じ座標に存在する、という事象が一度も起こらない確率を$\mod 998244353$で求めてください（注記参照）。
</p>

</section>

</div>

<div>

<section>

### **注記**

<p>
求める確率は必ず有理数となることが証明できます。またこの問題の制約下では、その値を互いに素な $2$つの整数 $P$, $Q$を用いて $\frac{P}{Q}$と表したとき、$R \times Q \equiv P\pmod{998244353}$かつ $0 \leq R \lt 998244353$を満たす整数 $R$がただ一つ存在することが証明できます。この $R$を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \leq K \leq 10$
</li>

<li>
$1 \leq N \leq 1000$
</li>

<li>
$0 \leq x_1 \lt x_2 \lt \cdots \lt x_K \leq 1000$
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

$K$$N$$x_1$$x_2$$\ldots$$x_K$
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

2 2
1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

374341633

</div>

<p>
求める確率は $\frac{5}{8}$です。
</p>

<p>
$374341633 \times 8 \equiv 5\pmod{998244353}$ですので、$374341633$を出力します。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

2 2
10 100

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
求める確率が $1$であることもあります。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10 832
73 160 221 340 447 574 720 742 782 970

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

553220346

</div>

</section>

</div>

</span>

</span>

</div>
