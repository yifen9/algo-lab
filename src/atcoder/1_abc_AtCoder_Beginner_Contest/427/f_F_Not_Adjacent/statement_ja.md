
<div>
﻿
<span>

<span>

<p>
配点 : $525$点
</p>

<div>

<section>

### **問題文**

<p>
長さ $N$の整数列 $A=(A _ 1,A _ 2,\ldots,A _ N)$が与えられます。
</p>

<p>
$A$の（連続するとは限らない）部分列は $2 ^ N$通りあります。
部分列 $(A _ {i _ 1},A _ {i _ 2},\ldots,A _ {i _ k})\ (1\le i _ 1\lt i _ 2\lt\cdots\lt i _ k\le N)$であって、次の $2$つの条件の両方を満たすものがいくつあるか求めてください。
</p>

<ul>

<li>
選ばれた要素は $A$において隣接しない。つまり、すべての $1\le j\lt k$に対して $1+i _ j\ne i _ {j+1}$が成り立つ。
</li>

<li>
総和が $M$の倍数である。つまり、$\displaystyle\sum _ {j=1} ^ kA _ {i _ j}\equiv0\pmod M$
</li>

</ul>

<p>
$2$つの部分列が整数列として等しくても、取り出す位置が異なるならそれら $2$つの部分列を区別して数えることに注意してください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le60$
</li>

<li>
$1\le M\le10 ^ 9$
</li>

<li>
$0\le A _ i\lt M$
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
入力は以下の形式で標準入力から与えられる。
</p>

<div>

$N$$M$$A _ 1$$A _ 2$$\ldots$$A _ N$
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

7 6
3 1 4 1 5 3 2

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
以下の $6$つの部分列が条件を満たします。
</p>

<ul>

<li>
$()=()$
</li>

<li>
$(A _ 1,A _ 3,A _ 5)=(3,4,5)$
</li>

<li>
$(A _ 1,A _ 4,A _ 7)=(3,1,2)$
</li>

<li>
$(A _ 1,A _ 6)=(3,3)$
</li>

<li>
$(A _ 2,A _ 5)=(1,5)$
</li>

<li>
$(A _ 3,A _ 7)=(4,2)$
</li>

</ul>

<p>
なので、`6`を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

15 10
5 5 5 5 5 5 5 5 5 5 5 5 5 5 5

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

798

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

20 998244353
778718481 719092922 676292280 713825156 0 434453766 620370916 67922064 0 577696866 21516423 955580612 955580612 0 332156721 0 0 0 632133714 500614291

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

40

</div>

</section>

</div>

</span>

</span>

</div>
