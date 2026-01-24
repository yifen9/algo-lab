
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
$N$人の研究者がおり、研究者には $1, 2, \ldots, N$の番号が付けられています。
</p>

<p>
研究者の間には $M$個の利害関係があり、$i = 1, 2, \ldots, M$に対して研究者 $A_i$と研究者 $B_i$は互いに利害関係にあります。
</p>

<p>
論文の査読者は、その論文の著者とは異なり、著者と利害関係にない相異なる $3$人の研究者である必要があります。
</p>

<p>
$i = 1, 2, \ldots, N$について以下の問題を解いてください。
</p>

<ul>

<li>
研究者 $i$が著者である論文の査読者の $3$人組として考えられるものは何通りあるか求めよ。
</li>

</ul>

<p>
ただし、すべての論文は単著であるものとします。
</p>

</section>

</div>

<div>

<section>

### **制約**

<ul>

<li>
$1 \leq N \leq 2 \times 10^5$
</li>

<li>
$0 \leq M \leq 2 \times 10^5$
</li>

<li>
$1 \leq A_i, B_i \leq N$
</li>

<li>
$A_i \neq B_i$
</li>

<li>
$i \neq j$のとき $(A_i, B_i) \neq (A_j, B_j)$
</li>

<li>
$i \neq j$のとき $(A_i, B_i) \neq (B_j, A_j)$
</li>

<li>
入力される値はすべて整数
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

$N$$M$$A_1$$B_1$$A_2$$B_2$$\vdots$$A_M$$B_M$
</div>

</section>

</div>

<div>

<section>

### **出力**

<p>
$i = 1, 2, \ldots, N$に対する答えをこの順に空白区切りで出力せよ。
</p>

</section>

</div>

</div>

---

<div>

<section>

### **入力例 1**

<div>

6 5
1 2
1 4
2 3
5 3
3 1

</div>

</section>

</div>

<div>

<section>

### **出力例 1**

<div>

0 1 0 4 4 10

</div>

<p>
以下、研究者の番号の集合により研究者の集合を表します。
</p>

<ul>

<li>

<p>
研究者 $1$が著者である論文の査読者の $3$人組として考えられるものはありません。
</p>

</li>

<li>

<p>
研究者 $2$が著者である論文の査読者の $3$人組として考えられるものは $\lbrace 4, 5, 6 \rbrace$の $1$通りです。
</p>

</li>

<li>

<p>
研究者 $3$が著者である論文の査読者の $3$人組として考えられるものはありません。
</p>

</li>

<li>

<p>
研究者 $4$が著者である論文の査読者の $3$人組として考えられるものは $\lbrace 2, 3, 5 \rbrace, \lbrace 2, 3, 6 \rbrace, \lbrace 2, 5, 6 \rbrace, \lbrace 3, 5, 6 \rbrace$の $4$通りです。
</p>

</li>

<li>

<p>
研究者 $5$が著者である論文の査読者の $3$人組として考えられるものは $\lbrace 1, 2, 4 \rbrace, \lbrace 1, 2, 6 \rbrace, \lbrace 1, 4, 6 \rbrace, \lbrace 2, 4, 6 \rbrace$の $4$通りです。
</p>

</li>

<li>

<p>
研究者 $6$が著者である論文の査読者の $3$人組として考えられるものは $\lbrace 1, 2, 3 \rbrace, \lbrace 1, 2, 4 \rbrace, \lbrace 1, 2, 5 \rbrace, \lbrace 1, 3, 4 \rbrace, \lbrace 1, 3, 5 \rbrace, \lbrace 1, 4, 5 \rbrace, \lbrace 2, 3, 4 \rbrace, \lbrace 2, 3, 5 \rbrace, \lbrace 2, 4, 5 \rbrace, \lbrace 3, 4, 5 \rbrace$の $10$通りです。
</p>

</li>

</ul>

</section>

</div>

---

<div>

<section>

### **入力例 2**

<div>

7 3
1 2
3 4
5 6

</div>

</section>

</div>

<div>

<section>

### **出力例 2**

<div>

10 10 10 10 10 10 20

</div>

</section>

</div>

---

<div>

<section>

### **入力例 3**

<div>

6 9
3 6
2 5
2 3
4 3
1 5
6 2
3 1
5 3
2 4

</div>

</section>

</div>

<div>

<section>

### **出力例 3**

<div>

1 0 0 1 0 1

</div>

</section>

</div>

</span>

</span>

</div>
