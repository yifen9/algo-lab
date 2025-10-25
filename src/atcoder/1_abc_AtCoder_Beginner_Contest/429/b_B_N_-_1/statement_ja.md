
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
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$と整数 $M$が与えられます。
</p>

<p>
$A$の $N$個の要素から $1$個を取り除くことで、残りの $N-1$個の要素の和をちょうど $M$にできるか判定してください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\le N\le 100$
</li>

<li>
$0\le M\le 10000$
</li>

<li>
$0\le A_i\le 100$
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

$N$$M$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$A$の $N$個の要素から $1$個を取り除くことで、残りの $N-1$個の要素の和をちょうど $M$にできる場合は `Yes`を、そうでない場合は `No`を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 10
3 2 3 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes

</div>

<p>
$A_1,A_3,A_4$を選ぶと総和は $3+3+4=10$となります。したがって、 `Yes`を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5 16
3 3 4 2 5

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

No

</div>

<p>
どのように $4$つの要素を選んでもその総和を $16$にすることはできません。したがって、 `No`を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

6 16
0 8 0 2 6 8

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

Yes

</div>

</section>

</div>

</span>

</span>

</div>
