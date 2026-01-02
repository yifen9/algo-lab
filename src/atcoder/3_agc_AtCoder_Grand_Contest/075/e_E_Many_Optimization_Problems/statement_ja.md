
<div>

<span>

<span>

<p>
配点 : $1600$点
</p>

<div>

<section>

### **問題文**

<blockquote>

<b>
Optimization Problem
</b>

<p>
長さ $N$の非負整数列 $A=(A_1,A_2,\dots,A_N)$が与えられます。また、長さ $N+1$の非負整数列 $X=(0,0,\dots,0)$があります。
</p>

<p>
あなたは今から $i=1,2,\dots,N$について以下の操作を行います。
</p>

<ul>

<li>
$0 \le v \le A_i$を満たす整数 $v$を選び、$X_i,X_{i+1}$にそれぞれ $v,A_i-v$を加算する。
</li>

</ul>

<p>
操作終了時の $X$の最大値としてあり得る値の最小値を求めてください。

</p>

</blockquote>

<p>
正整数 $N,M$と素数 $P$が与えられます。長さ $N$かつ総和が $M$であるような非負整数列 $A=(A_1,A_2,\dots,A_N)$全てに対する 
<b>
Optimization Problem
</b>
の答えの総和を $P$で割った余りを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \le N \le 100$
</li>

<li>
$1 \le M \le 10^{18}$
</li>

<li>
$9 \times 10^8 \le P \le 10^9$
</li>

<li>
$P$は素数
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

$N$$M$$P$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>

<b>
Optimization Problem
</b>
の答えの総和を $P$で割った余りを出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

3 3 998244353

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

13

</div>

<p>
例えば、$A=(1,0,2)$について 
<b>
Optimization Problem
</b>
を解きます。例えば、操作列の一例として以下のようなものがあります。
</p>

<ul>

<li>
$i = 1$では $v = 1$とする。$X=(1,0,0,0)$となる。
</li>

<li>
$i = 2$では $v = 0$とする。$X=(1,0,0,0)$となる。
</li>

<li>
$i = 3$では $v = 1$とする。$X=(1,0,1,1)$となる。
</li>

</ul>

<p>
$X$の最大値を $0$以下にすることは出来ないため、答えは $1$です。
</p>

<p>
これ以外に答えが $1$となる数列が $6$個、答えが $2$となる数列が $3$個あるためその総和は $13$です。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

10 135 998244353

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

679877945

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

100 1000000000000000000 924844033

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

789282612

</div>

</section>

</div>

</span>

</span>

</div>
