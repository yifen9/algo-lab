
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
長さ $N$の正整数列 $A=(A_1,A_2,\ldots,A_N)$に対して，$Q$回の操作を行います．$1\leq q\leq Q$に対して，$q$回目の操作の情報は正整数 $i_q, x_q$（ただし $1\leq i_q\leq N$）として与えられ，その内容は $A_{i_q}$に $x_q$を加算するというものです．
</p>

<p>
あなたの目標は，$A$の初期状態を適切に定めることで，どの時点においても（つまり，初期状態および各操作の直後においても）以下の条件が成り立つようにすることです．
</p>

<ul>

<li>
$0<A_1 < A_2 < \cdots < A_N$が成り立つ．
</li>

</ul>

<p>
この目標を達成するとき，$A$の初期状態における要素の総和として考えられる最小値を求めてください．
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$2\leq N\leq 2\times 10^5$
</li>

<li>
$1\leq Q\leq 2\times 10^5$
</li>

<li>
$1\leq i_q\leq N$
</li>

<li>
$1\leq x_q\leq 10^5$
</li>

<li>
入力される値はすべて整数．
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
入力は以下の形式で標準入力から与えられます．
</p>

<div>

$N$$Q$$i_1$$x_1$$\vdots$$i_Q$$x_Q$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
目標を達成するとき，$A$の初期状態における要素の総和として考えられる最小値を出力してください．
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

4 2
1 2
2 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

22

</div>

<p>
初期状態の $A$が $A=(1,4,8,9)$であったとします．このとき，
</p>

<ul>

<li>
$1$回目の操作直後の $A$：$A=(3,4,8,9)$
</li>

<li>
$2$回目の操作直後の $A$：$A=(3,7,8,9)$
</li>

</ul>

<p>
となり，どの時点においても $A$は条件を満たしていることが確かめられます．
</p>

<p>
この場合，$A$の初期状態における要素の総和は $\displaystyle \sum_{i=1}^NA_i=1+4+8+9=22$です．
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

4 2
2 3
1 2

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

100000 1
1 100000

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

14999950000

</div>

</section>

</div>

</span>

</span>

</div>
