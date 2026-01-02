
<div>

<span>

<span>

<p>
配点 : $300$点
</p>

<div>

<section>

### **問題文**

<p>
$N$個のドミノが数直線上に一列に並んでいます。$i$番目のドミノは座標 $i$の位置に立っており、高さは $A_i$です。
</p>

<p>
$i$番目のドミノが右に倒れると、座標 $i$以上 $i+A_i$未満の範囲にあるドミノが全て右に倒れます。
</p>

<p>
$1$番目のドミノを右に倒したとき、全部でいくつのドミノが倒れますか？
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\leq N \leq 5\times 10^5$
</li>

<li>
$1\leq A_i \leq N$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$1$番目のドミノを右に倒したときに倒れるドミノの個数を出力せよ。
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
3 1 4 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

4

</div>

<p>
$1$番目のドミノが右に倒れると、$2,3$番目のドミノも右に倒れます。$3$番目のドミノが右に倒れると、$4$番目のドミノも倒れます。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

9
1 4 1 4 2 1 3 5 6

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
$1$番目のドミノを右に倒しても、他のドミノが倒れることはありません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

10
5 4 3 2 1 1 2 3 4 5

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
