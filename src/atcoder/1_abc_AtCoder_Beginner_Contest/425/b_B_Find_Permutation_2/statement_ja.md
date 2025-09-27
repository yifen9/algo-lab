
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
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます。ここで、 $A$の各要素は $-1$または $1$以上 $N$以下の整数です。
</p>

<p>
以下の条件を全て満たす長さ $N$の整数列 $P=(P_1,P_2,\ldots,P_N)$が存在するか判定し、存在するならば一つ求めてください。
</p>

<ul>

<li>
$P$は $(1,2,\ldots,N)$を並び替えてできる整数列である。
</li>

<li>
$i=1,2,\ldots,N$に対し、 $A_i \neq -1$ならば $P_i=A_i$が成り立つ。
</li>

</ul>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le 10$
</li>

<li>
$A_i=-1$または $1\le A_i \le N$
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

$N$$A_1$$A_2$$\ldots$$A_N$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
条件を全て満たす $P$が存在しない場合は `No`と出力せよ。
</p>

<p>
そうでない場合、条件を全て満たす $P$を以下の形式で出力せよ。
</p>

<div>

Yes
$P_1$$P_2$$\ldots$$P_N$
</div>

<p>
条件を全て満たす $P$が複数存在する場合、どれを出力しても正答となる。
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
-1 -1 2 -1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

Yes
3 1 2 4

</div>

<p>
$P=(3,1,2,4)$とすると条件を全て満たします。
</p>

<p>
このほかにも、 $P=(1,3,2,4)$や $P=(4,3,2,1)$なども条件を全て満たします。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5
-1 -1 1 -1 1

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
条件を全て満たす $P$は存在しません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

7
3 -1 4 -1 5 -1 2

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

Yes
3 7 4 1 5 6 2

</div>

</section>

</div>

</span>

</span>

</div>
