
<div>

<span>

<span>

<p>
配点 : $1100$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の `A`, `B`, `C`からなる文字列 $S$のうち、以下の値が $K$になるものの個数を $998244353$で割った余りを求めてください。
</p>

<ul>

<li>
$S$の(連続とは限らない)部分列のうち、(連続とは限らない)部分列として `ABC`を含まないものの長さの最大値
</li>

</ul>

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
$1 \le N \le 10^6$
</li>

<li>
$\max(0,N-100) \le K \le N$
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
各ケースは以下の形式で与えられる。
</p>

<div>

$N\ K$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。$i(1 \le i \le T)$行目には、$i$番目のテストケースの答えを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4
4 3
8 6
123 100
123456 123400

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

9
462
741573397
255048895

</div>

<p>
$1$番目のテストケースについて、例えば `ACBC`は条件を満たします。`ACBC`自身は部分列に `ABC`を含み、`ACC`は部分列に `ABC`を含まないため、部分列に `ABC`を含まないような部分列の長さの最大値は $3$となります。
他にも `AABC`, `ABCA`などが条件を満たします。
</p>

</section>

</div>

</span>

</span>

</div>
