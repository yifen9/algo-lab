
<div>

<span>

<span>

<p>
配点 : $700$点
</p>

<div>

<section>

### **問題文**

<p>
$(1,2,\ldots,N)$の順列 $P$と、空の配列 $A$があります。
$P$に対して以下の操作を $N-1$回行います。
</p>

<ul>

<li>
隣接する $2$要素を選ぶ。選んだうち小さい方の要素を $P$から削除し、削除した要素の前後を結合する。削除した要素を $A$の末尾に追加する。
</li>

</ul>

<p>
最終的にできる長さ $N-1$の数列 $A$としてあり得るものの数を $998244353$で割ったあまりを求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2 \le N \le 2\times 10^5$
</li>

<li>
$1 \le P_i \le N$
</li>

<li>
$P$は $(1,2,\ldots,N)$の順列
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

$N$$P_1$$P_2$$\ldots$$P_N$
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

4
1 2 3 4

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

6

</div>

<p>
最終的な $A$としては $(1,2,3)$の順列 $6$通りの全てがあり得ます。
</p>

<p>
例えば、$A=(2,1,3)$とする操作手順は以下の通りです。
</p>

<ul>

<li>
$2,3$を選ぶ。$2$が削除され、$P=(1,3,4), A=(2)$となる。
</li>

<li>
$1,3$を選ぶ。$1$が削除され、$P=(3,4), A=(2,1)$となる。
</li>

<li>
$3,4$を選ぶ。$3$が削除され、$P=(4), A=(2,1,3)$となる。
</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3
3 1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

1

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

24
10 24 3 4 8 14 5 2 22 9 21 1 15 6 13 23 18 12 7 17 19 16 20 11

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

303178128

</div>

</section>

</div>

</span>

</span>

</div>
