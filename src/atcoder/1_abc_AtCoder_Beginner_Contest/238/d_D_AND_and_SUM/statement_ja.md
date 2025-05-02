
<div>

<span>

<span>

<p>
配点 : $400$点
</p>

<div>

<section>

### **問題文**

<p>
$T$個のテストケースについて、以下の問題を解いてください。
</p>

<blockquote>

<p>
非負整数 $a,s$が与えられます。以下の条件を両方とも満たす非負整数の組 $(x,y)$は存在しますか？
</p>

<ul>

<li>
$x\ \text{AND}\ y=a$
</li>

<li>
$x+y=s$
</li>

</ul>

</blockquote>

<details>

<summary>
$\text{AND}$とは
</summary>

<p>
非負整数 $n, m$の bit ごとの論理積 $n\ \text{AND}\ m$は、以下のように定義されます。

</p>

<ul>

<li>
$n\ \text{AND}\ m$を二進表記した際の $2^k \, (k \geq 0)$の位の数は、$n, m$を二進表記した際の $2^k$の位の数のうち
<b>
両方
</b>
が $1$であれば $1$、そうでなければ $0$である。
</li>

</ul>
例えば、$4\ \text{AND}\ 6 = 4$となります（二進表記すると: $100\ \text{AND}\ 110 = 100$）。

<p>

</p>

</details>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq T \leq 10^5$
</li>

<li>
$0 \leq a,s \lt 2^{60}$
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
入力は標準入力から与えられる。入力の $1$行目は以下の形式である。
</p>

<div>

$T$
</div>

<p>
その後、 $T$個のテストケースが続く。各テストケースは以下の形式で与えられる。
</p>

<div>

$a$$s$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$T$行出力せよ。$i\ (1 \leq i \leq T)$行目には、$i$番目に与えられるテストケースについて問題文中の条件を両方とも満たす非負整数の組 $(x,y)$が存在するなら `Yes`を、存在しないなら `No`を出力せよ。
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
1 8
4 2

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes
No

</div>

<p>
$1$番目のテストケースにおいては、$(x,y)=(3,5)$などが条件を満たします。
</p>

<p>
$2$番目のテストケースにおいては、条件を満たす非負整数の組 $(x,y)$は存在しません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4
201408139683277485 381410962404666524
360288799186493714 788806911317182736
18999951915747344 451273909320288229
962424162689761932 1097438793187620758

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

No
Yes
Yes
No

</div>

</section>

</div>

</span>

</span>

</div>
