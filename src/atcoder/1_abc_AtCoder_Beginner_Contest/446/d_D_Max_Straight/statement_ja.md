
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
長さ $N$の整数列 $A=(A_1,A_2,\ldots,A_N)$が与えられます。
</p>

<p>
整数列 $A$の部分列 $B=(B_1,B_2,\ldots,B_{|B|})$であって、以下の条件を満たすものの長さの最大値を求めてください。
</p>

<ul>

<li>
全ての $1\le i\le |B| - 1$を満たす整数 $i$に対し、 $B_i+1=B_{i+1}$が成り立つ。
</li>

</ul>

<details>

<summary>
部分列とは
</summary>
数列 $A$の部分列とは、$A$の要素を $0$個以上選んで削除し、残った要素を元の順序を保って並べた数列のことを指します。

</details>

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
$1\le A_i\le 10^9$
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

7
3 4 3 5 7 6 2

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
$B=(3,4,5,6)$は $A$の部分列であり条件を満たし、その長さは $4$です。
</p>

<p>
条件を満たす部分列であって長さが $4$より長いものは存在しないので、 $4$を出力してください。
</p>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

5
5 4 3 2 1

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

10
1 2 3 4 5 6 7 8 9 10

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

10

</div>

</section>

</div>

</span>

</span>

</div>
