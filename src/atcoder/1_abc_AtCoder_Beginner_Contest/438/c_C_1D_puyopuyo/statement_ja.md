
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
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます。
</p>

<p>
あなたは以下の操作を $0$回以上好きな順番で好きな回数行うことができます：
</p>

<ul>

<li>
$A_k=A_{k+1}=A_{k+2}=A_{k+3}$を満たす $1$以上 $|A|-3$以下の整数 $k$を選び、$A$から $A_k,A_{k+1},A_{k+2},A_{k+3}$を削除する。（より厳密には、 $A$を $(A_1,A_2,\ldots,A_{k-1},A_{k+4},A_{k+5},\ldots,A_N)$に置き換える。）
</li>

</ul>

<p>
ここで、 $|A|$は整数列 $A$の長さを表します。
</p>

<p>
操作を繰り返した後の最終的な $|A|$としてあり得る最小値を求めてください。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1\le N\le 2\times 10^5$
</li>

<li>
$1\le A_i\le N$
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
操作を繰り返した後の最終的な $|A|$としてあり得る最小値を出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

10
1 1 1 4 4 4 4 1 2 3

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

2

</div>

<p>
以下のように $2$回操作することで $|A|=2$にすることができます。
</p>

<ul>

<li>
$k=4$を選ぶ。$A_4=A_5=A_6=A_7=4$が成り立つためこの選択は正当である。 $A=(1,1,1,1,2,3)$となる。
</li>

<li>
$k=1$を選ぶ。$A_1=A_2=A_3=A_4=1$が成り立つためこの選択は正当である。 $A=(2,3)$となる。
</li>

</ul>

<p>
$|A|$を $2$未満にすることはできないため、 $2$を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

3
2 1 3

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

3

</div>

<p>
はじめから操作を行うことができません。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

13
1 1 4 4 4 1 1 1 1 4 1 4 1

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
